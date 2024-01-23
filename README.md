## ansible_project

#Déploiement automatique avec Ansible

#Introduction :
Le but de ce projet est de déployer un réseau en découvrant deux outils modernes mis à  disposition des administrateurs système. Ces outils sont également utilisés dans les milieux  industriels lors de développements et de tests. cette partie propose un déploiement  automatique en utilisant Ansible dans un environnement Linux natif (pas de conteneurs)
#I - Ansible :
Une start-up a besoin de concevoir et mettre en place son parc informatique. L’entreprise est  distribuée géographiquement sur deux sites. L’installation des services se fera par déploiement  automatique à l’aide d’Ansible.  
On se propose de créer 4 machines virtuelles (2 par sites) dans lesquelles les services seront  installés. La distribution utilisée est Debian. On suppose qu’en réalité, des centaines de machines  doivent être administrés (et il faut donc automatiser au maximum les déploiement / la  maintenance). 
Les besoins sont les suivants : 
⚫ Mise en place d’un serveur DHCP (un par site). 
⚫ Mise en place d’un serveur DNS (un par site). 
⚫ VPN pour interconnecter les deux sites.  
⚫ Un NFS public et privé (pour chaque utilisateur) doit être disponible sur l’ensemble du  réseau.  
⚫ Une gestionnaire de dépôt GIt soit être mis en place.  
⚫ Un serveur Apache.  
⚫ L’authentification générale (ssh, git, etc …) se fait via LDAP. 
⚫ La mise à jour de tous les systèmes doit se faire en une commande Ansible. 
Toute l’installation doit s’effectuer via Ansible, de sorte que l’ajout d’un noeud dans le cluster doit  se faire entièrement automatiquement en seulement quelques lignes de commandes. 
A noter: on peut avantageusement utiliser Ansible pour ses propre besoins personnels; par  exemple afin de déployer son propre environnement de travail à la suite d’une installation fraîche  d’une distribution Linux sur une machine unique ...
