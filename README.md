# Simulation de l’interaction entre 4 molécules HTX et l’ADN

<p align="justify">
Pour comprendre comment la molécule HTX interagit avec l’ADN, il est possible de simuler un fragment de deux brins d’ADN formant une double hélice et 4 molécules dans l’eau et observer comment les molécules interagissent.
</p>
<p align="justify">
Dans la méthode utilisée, les atomes sont des boules reliées par des ressorts qui représentent les liaisons chimiques fortes. Les interactions chimiques faibles sont reproduites grâce aux propriétés des boules. Cette approche, appelée méthode « classique », permet de simuler le comportement de plusieurs centaines de milliers d’atomes pour des durées allant de la dizaine de nanosecondes à quelques microsecondes.
</p>
<p align="justify">
Ici, on va regarder une trajectoire de 200 ns avec un logiciel de visualisation appelé VMD. Les molécules d’eau ont été retirées pour faciliter la visualisation.
</p>

## Tutoriel

1.	Ouvrir VMD

2.	Télécharger le dossier `center_dsDNA_4htx.zip` disponible sur cette page GitHub. Le décompresser pour obtenir le fichier contenant la trajectoire : `center_dsDNA_4htx.pdb`.

3.	Charger la trajectoire : File --> new molecule

<img width="1199" height="605" alt="Screenshot 2026-06-11 at 15 14 36" src="https://github.com/user-attachments/assets/f49c5dac-8b53-4b7c-9344-b285b13aef92" />

4.	Seules les liaisons des atomes apparaissent.

<img width="1034" height="1056" alt="Screenshot 2026-06-11 at 15 20 06" src="https://github.com/user-attachments/assets/9f1e0447-e3db-487c-8d9d-a61dd72582ee" />

On peut modifier la représentation : Graphics --> representation

<img width="562" height="359" alt="Screenshot 2026-06-11 at 15 35 27" src="https://github.com/user-attachments/assets/b803fb5a-efba-4252-8607-aa8dd5b0fe62" />

Sélectionner « nucleic » ; Drawing method  « new ribbon » ; coloring methods « Resname », qui permet de colorer en fonction des bases nucléiques :<br>
Adenine : rose  Thymine : blanc<br>
Guanine : vert  Cytosine : vert clair<br>
Autres couleurs : bases nucléiques aux extrémités.

<img width="1316" height="1022" alt="Screenshot 2026-06-11 at 15 28 54" src="https://github.com/user-attachments/assets/0db6ee45-c55c-461b-a179-e39a56483f51" />

Créer une nouvelle représentation :<br>
Sélectionner « resname HTX » ; Drawing method « CPK » : chaque atome est représenté par une boule (cyan = carbone, bleu = azote, rouge = oxygène, blanc=hydrogène).

<img width="1108" height="873" alt="Screenshot 2026-06-11 at 15 33 23" src="https://github.com/user-attachments/assets/d9cd15ca-fdc8-4375-9de8-231e55d9a4a3" />

Pour faciliter les observations, on peut faire les modifications suivantes dans Display : choisir Orthographic, enlever le depth Cueing.

5.	Observer la trajectoire et regarder ce qui se passe.

<img width="789" height="456" alt="Screenshot 2026-06-11 at 15 38 55" src="https://github.com/user-attachments/assets/e03e25d1-264d-49e1-8b59-7d7dc93e1cb5" />

## Questions

-	D’où partent les molécules ? 
-	Vont-elles interagir avec l’ADN ? Si oui, où ? Au bout de combien de temps de simulation ? Les interactions durent elles « longtemps » ?
-	Les interactions ont-elles un impact sur la structure de l’ADN ?
