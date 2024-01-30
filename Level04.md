Pour commencer, il faut aller dans le dossier "04_kwisatz"
```cd
cd /home/level/04_kwisatz
```
Dans ce dossier, il y a un seul fichier "README.nfo" qui dit:"Look in your ~"
```cd
cd ~
```
Arrivé là bas, on va naviguer dans des dossiers
```cd
cd ~/level/04_kwisatz 
```
Dedans il y a deux fichiers : "README.txt" et "README2.md". On va d'abord afficher le contenu de README.txt
```cat
cat README.txt
```
Et on peut voir :"I wrote you an important message in README2.md". On va alors afficher le contenu de "README2.md"
```cat
cat README2.md
```
Mais il dit qu'on n'a pas la permission pour afficher ce contenu. Et on va devoir modifier le gestion de permission pour ce fichier
```mod
chmod +r README2.md
```
Après celà on refait
```cat
cat README2.md
```
Et on obtient le mot de passe
