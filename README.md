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

<img width="995" height="997" alt="Screenshot 2026-06-11 at 15 16 58" src="https://github.com/user-attachments/assets/52c69a46-5d47-49c5-a46d-3815cb4b2d8b" />

On peut modifier la représentation : Graphics --> representation

<img width="354" height="178.5" alt="Picture 2" src="https://github.com/user-attachments/assets/3fe4a177-3a7e-4678-b637-26bb1c809964" />

Sélectionner « nucleic » ; Drawing method  « new ribbon » ; coloring methods « Resname », qui permet de colorer en fonction des bases nucléiques :
Adenine : rose		Thymine : blanc
Guanine : vert		Cytosine : vert clair	
Autres couleurs : bases nucléiques aux extrémités.

<img width="501" height="390" alt="image" src="https://github.com/user-attachments/assets/1a961114-3708-48d5-8d79-1b43b16c32c3" />

Créer une nouvelle représentation
Sélectionner « resname HTX » ; Drawing method « CPK » : chaque atome est représenté par une boule (cyan = carbone, bleu = azote, rouge = oxygène, blanc=hydrogène).

<img width="681" height="480" alt="image" src="https://github.com/user-attachments/assets/2175d852-806f-4fa6-b09b-6ffb72e8221a" />

Pour faciliter les observations, on peut faire les modifications suivantes dans Display : choisir Orthographic, enlever le depth Cueing.

5.	Observer la trajectoire et regarder ce qui se passe.

<img width="555" height="219" alt="image" src="https://github.com/user-attachments/assets/0f275180-ab5c-4e9a-b190-ccf7b820a2d1" />

## Questions

-	D’où partent les molécules ? 
-	Vont-elles interagir avec l’ADN ? Si oui, où ? Au bout de combien de temps de simulation ? Les interactions durent elles « longtemps » ?
-	Les interactions ont-elles un impact sur la structure de l’ADN ?
