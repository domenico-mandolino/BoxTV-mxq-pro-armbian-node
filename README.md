MXQ Pro (S905W) – Armbian Linux Node

Ce dépôt documente la transformation d’un boîtier TV Android MXQ Pro, basé sur un SoC Amlogic S905W, en un nœud Linux headless destiné à un usage homelab / réseau.

À l’origine conçu pour exécuter Android TV, ce type de matériel est aujourd’hui largement obsolète pour son usage initial. L’objectif de ce projet est de revaloriser ce boîtier en l’intégrant dans une infrastructure personnelle orientée services réseau, en particulier comme futur point d’accès VPN.

Ce dépôt s’inscrit dans une démarche pédagogique et pratique, visant à :

- comprendre les contraintes des architectures ARM low-cost,

- manipuler les mécanismes de boot (u-boot, device tree),

- diagnostiquer et résoudre des problèmes système réels,

- documenter un processus technique de bout en bout.

Le système retenu est Armbian (Debian Bookworm), choisi pour sa stabilité, sa compatibilité avec les usages serveur et sa cohérence avec le reste du homelab (notamment un serveur Proxmox documenté dans un dépôt séparé).

Le projet couvre :

l’identification du matériel (S905W),

les différentes méthodes de boot et de flash possibles,

le choix de l’OS en fonction des objectifs futurs,

les difficultés rencontrées lors de l’installation,

la résolution de problèmes critiques (alimentation, boot, SSH),

l’obtention d’un accès distant fonctionnel et stable.

L’ensemble du travail présenté ici correspond à un retour d’expérience complet.
Les captures d’écran, photos du matériel et étapes détaillées sont regroupées dans un document PDF complémentaire, publié séparément.

Ce dépôt constitue la première étape d’un projet plus large.
Un second dépôt sera consacré à la mise en place d’un VPN (WireGuard) sur ce même boîtier, une fois la base système validée.
