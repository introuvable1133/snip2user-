Discord Username Availability Checker & Reservation System
Overview
Ce projet est un outil d'automatisation réseau conçu pour surveiller la disponibilité et procéder à l'attribution de noms d'utilisateurs courts (formats 3 lettres et 4 caractères). Développé dans un objectif de performance et de haute concurrence, le système s'appuie sur une architecture asynchrone couplée à une gestion distribuée de requêtes via mandataires (proxys).

Architecture et Spécifications Techniques
Traitement Asynchrone et Concurrence : Utilisation d'un modèle d'entrées/sorties non bloquant permettant d'exécuter un volume élevé de requêtes par seconde sans engorgement système.

Gestion et Rotation des Proxys : Prise en charge des protocoles HTTP, HTTPS, SOCKS4 et SOCKS5. Le module intègre une rotation automatique des adresses IP afin de répartir la charge, de contourner les limitations de débit (rate limiting) et d'atténuer les blocages réseau.

Filtrage et Validation de Formats : Moteur de génération et de filtrage ciblant spécifiquement les combinaisons rares (chaînes de 3 caractères alphabétiques et 4 caractères alphanumériques).

Système d'Alerting et Logging : Traçabilité complète des statuts HTTP (codes 200, 429, etc.) et intégration de webhooks pour la notification en temps réel dès qu'une opération aboutit.
