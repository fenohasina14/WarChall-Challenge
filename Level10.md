Comme dans tous les autres niveaux il suffit d'aller dans le fichier du niveau
```cd
cd /home/level/10_choose_your_path
```
On verra alors qu'il y a 4 fichiers : "charp", "charp.c","compile.sh" et enfin "solution.txt". On va essayer de voir le contenu de "solution.txt" mais il dit qu'on n'a pas l'autorisation de faire ça.

Et utiliser "chmod" ne changera rien
Il faut alors voir le contenu des autres dossiers. Et on peut voir que ces derniers sont tous des scripts mais c'est seulement "charp" qui est éxécutable et ce dernier à besoin d'un fichier comme argument
```exc
./charp solution.txt
```
On constate que ce script sert à compter les caractères par ligne. Le script peut donc voir le contenu de "solution.txt" et on peut profiter de celà

Pour faire celà, on va exploiter quelque faille de Linux tel que le dossier tmp qui est un cache temporaire pour des fichiers
On va combiner deux commandes à la fois qui va contourner la sécurité en exploitant les failles
```exc
./charp "solution.txt | cp solution.txt tmp/newFile.txt"
```
après celà nous pourrons alors voir le contenu de solution.tx qui a été copié dans newFile.txt
```cat
cat tmp/newFile.txt
```
Et on a le mot de passe
