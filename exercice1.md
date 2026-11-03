1. Système d’exploitation
Un système d’exploitation est un ensemble de programmes qui sert d’intermédiaire entre le matériel et les applications, et qui gère les ressources de la machine. Trois ressources gérées : le processeur (temps CPU), la mémoire (RAM), les disques et le stockage. On peut aussi citer les périphériques d’entrée/sortie et le réseau.

2. Noyau, shell, applications

Noyau (kernel) : cœur du système. Il gère les processus, la mémoire, les périphériques et le système de fichiers, et il dialogue directement avec le matériel.
Shell : interpréteur de commandes. Il reçoit les commandes de l’utilisateur et les transmet au noyau.
Applications : programmes utilisés par l’utilisateur (navigateur, éditeur, serveur web…).

Les applications doivent obligatoirement passer par le noyau (via les appels système) pour accéder au matériel.

3. Multitâche et multiutilisateur

Multitâche : plusieurs processus s’exécutent en apparence en même temps, le noyau se partageant le temps du processeur entre eux.
Multiutilisateur : plusieurs utilisateurs peuvent travailler simultanément sur la machine, chacun avec son compte, ses fichiers et ses droits, isolés des autres.

4. Le 1er janvier 1970
C’est l’Epoch (00:00:00 UTC). Les concepteurs d’UNIX (Bell Labs) l’ont choisie comme origine arbitraire, proche de la naissance du système. Le temps est ensuite compté en secondes écoulées depuis cette date, ce qui est simple à stocker et à calculer.

5. Distribution GNU/Linux
Une distribution est un ensemble cohérent composé du noyau Linux, des outils GNU, de logiciels, d’un installateur et d’un gestionnaire de paquets, maintenu et publié par une communauté ou une entreprise.

Communautaires : Debian, Fedora (ou Arch, Rocky Linux).
Commerciales : Red Hat Enterprise Linux (RHEL), SUSE Linux Enterprise.

6. « Libre ne veut pas dire gratuit »
« Libre » désigne la liberté d’utiliser, d’étudier, de modifier et de redistribuer le logiciel, et non son prix. Un logiciel libre peut être vendu (support, distribution commerciale), et un logiciel gratuit peut être propriétaire (freeware).

Les quatre libertés de la GPL :

Liberté 0 : exécuter le programme, pour n’importe quel usage.
Liberté 1 : étudier son fonctionnement et l’adapter (accès au code source).
Liberté 2 : redistribuer des copies.
Liberté 3 : améliorer le programme et publier ses modifications.

7. Analyse de ls -lia /etc /home

Commande : ls
Options : -l, -i, -a (regroupées en -lia)
Arguments : /etc et /home
Sans regroupement : ls -l -i -a /etc /home

8. -l et --list, et le double tiret seul
-l est une option courte (un tiret, une lettre, regroupable avec d’autres). --list est une option longue (deux tirets, un mot complet, plus lisible, non regroupable).
Le double tiret -- seul marque la fin des options : tout ce qui suit est traité comme un argument, même s’il commence par -. Exemple : rm -- -test.

9. Les invites

$ : session en utilisateur ordinaire.
# : session en root (administrateur).

10. Commandes

a. man 5 passwd
b. man -k clear (ou apropos clear)
c. shutdown -h +15 "Maintenance" (ou shutdown -P +15 "Maintenance")
d. reboot (ou shutdown -r now)
e. !! (ou la flèche ↑)
f. !ls
g. history -c. Cette commande efface l’historique de la session en cours, mais pas ~/.bash_history, qu’il faut réécrire avec history -w.