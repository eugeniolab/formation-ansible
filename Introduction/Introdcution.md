Introduction à Ansible

Qu'est-ce qu'Ansible ?
Ansible est un moteur d'automatisation informatique open source qui permet d'automatiser :

Le provisionnement : Installation et configuration initiale des ressources (serveurs, machines virtuelles, conteneurs, etc.).
La gestion de la configuration : Maintien de la cohérence des systèmes en appliquant des paramètres spécifiques (fichiers de configuration, services, utilisateurs, etc.).
Le déploiement des applications : Installation et mise à jour des applications sur plusieurs environnements de manière fiable et reproductible.
L'orchestration : Coordination et enchaînement des différentes tâches et services dans un environnement distribué.
De nombreux autres processus informatiques : Sauvegardes, mises à jour, gestion des utilisateurs, surveillance, et bien plus encore.
Il est gratuit et bénéficie de l'expertise et de l'intelligence collective de milliers de contributeurs.

Comment fonctionne Ansible ?
Ansible est sans agent (agentless), ce qui signifie qu'il n'est pas nécessaire d'installer un logiciel sur les nœuds gérés.

Pour automatiser Linux et Windows, Ansible se connecte aux nœuds gérés et y envoie de petits programmes appelés modules Ansible. Ces programmes sont conçus pour représenter un modèle de ressources correspondant à l'état souhaité du système. Ansible exécute ensuite ces modules (par défaut via SSH) et les supprime une fois l'opération terminée. Ces modules sont conçus pour être idempotents lorsque cela est possible, ce qui signifie qu'ils n'apportent des modifications au système que lorsque cela est nécessaire.

Pour l'automatisation des équipements réseau et autres appareils informatiques où l'exécution de modules est impossible, Ansible fonctionne depuis le nœud de contrôle. Étant sans agent, Ansible peut toujours communiquer avec ces appareils sans nécessiter l'installation d'une application ou d'un service sur le nœud géré.
