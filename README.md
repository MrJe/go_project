# go_project
Création d'un goban, gestion de la pose des pierres, calculs des points

/* ************************************************************************** */
### AFFICHAGE DU GOBAN

- La taille doit être > 1 && < 100;
- Les coordonnées doivent être affichées;

Voici un exemple d'affichage d'un goban 9 * 9 :
```
   1  2  3  4  5  6  7  8  9
1  .  .  .  .  .  .  .  .  .
2  .  .  .  .  .  .  .  .  .
3  .  .  .  .  .  .  .  .  .
4  .  .  .  .  .  .  .  .  .
5  .  .  .  .  .  .  .  .  .
6  .  .  .  .  .  .  .  .  .
7  .  .  .  .  .  .  .  .  .
8  .  .  .  .  .  .  .  .  .
9  .  .  .  .  .  .  .  .  .
```

/* ************************************************************************** */
### POSE DES PIERRES

- Les pierres sont noires 'x' et blanches 'o';
- Noir commence et les joueurs jouent chacun leur tour;
- Pour jouer une pierre, le joueur doit donner les coordonnées sous la forme : ligne-colonne;
- La grille est actualisée et affichée après chaque coup;
- Le nombre de pierres capturées est indiquée sous la grille;

Voici un exemple d'affichage en cours de partie :
```
   1  2  3  4  5  6  7  8  9
1  .  .  .  .  .  .  .  .  .
2  .  .  .  .  .  .  .  .  .
3  .  .  x  .  .  .  o  .  .
4  .  .  .  .  .  x  .  .  .
5  .  x  .  .  .  .  .  .  .
6  .  .  .  .  .  .  .  .  .
7  .  .  o  .  .  .  o  .  .
8  .  .  .  .  .  .  .  .  .
9  .  .  .  .  .  .  .  .  .

prisonners > x : 0 | o : 0
```

/* ************************************************************************** */
### CALCUL DES POINTS

- Lorsque les deux joueurs passent consécutivement, la partie est terminée;
- Le décompte se fait automatiquement et le résultat s'affiche sous la grille;

Voici un exemple de fin de partie :
```
   1  2  3  4  5  6  7  8  9
1  .  .  .  .  o  x  x  .  .
2  .  .  .  .  o  o  x  .  .
3  .  .  .  o  .  o  x  .  .
4  .  o  x  o  .  o  x  .  .
5  .  o  o  x  o  .  o  x  .
6  .  o  x  x  o  o  o  x  .
7  o  o  o  x  o  x  x  .  .
8  o  x  x  x  x  .  .  .  .
9  x  x  .  x  .  .  .  .  .

prisonners > x : 1 | o : 1

result > x = 22 + 1 | o = 18 + 2
result > x = 23 | o = 20
result > x win by 3 points
```

/* ************************************************************************** */
### ADD ON

- [ ] sauvegarde du kifu dans un fichier txt (liste des coups joués);
- [ ] changement des symboles utilisés pour les pierres;
- [ ] lister les x derniers coups sur la droite du plateau;

Test d'une ligne;<br />
Ceci est une seconde ligne;<br />
Voilà la dernière
