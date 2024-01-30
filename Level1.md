Pour ce prochain niveau, il faut tout d'abord naviguer vers le dossier 02 avec la commande
```cd
cd /home/level/02
```
Arrivé là, on peut voir deux dossiers et aucun d'eux ne semble contenir le fichier contenant le mot de passe. On doit alors voir si il y a des dossiers cachés avec la commande
```ls
ls -a
```
Il y a bel et bien un dossier caché nommé ".porb" et il suffit d'aller dans ce dernier avec la commande
```cd
cd .porb/
```
Et encore une fois il n'y a rien et on doit donc voir les dossiers cachés avec un coup de 
```ls
ls -a
```
On voit un fichier caché nommé ".solution" et il suffit d'afficher le contenu de ce dossier
```cat
cat .solution
```
Et on obtient le mot de passe
