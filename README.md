# Simulation de l’interaction entre 4 molécules HTX et l’ADN

Pour comprendre comment la molécule interagit avec l’ADN, il est possible de simuler un fragment de deux brins d’ADN formant une double hélice et 4 molécules dans l’eau et observer comment les molécules interagissent. 
Dans la méthode utilisée, les atomes sont des boules reliées par des ressorts qui représentent les liaisons chimiques fortes. Les interactions chimiques faibles sont reproduites grâce aux propriétés des boules. Cette approche, appelée méthode « classique », permet de simuler le comportement de plusieurs centaines de milliers d’atomes pour des durées allant de la dizaine de nanosecondes à quelques microsecondes.
Ici, on va regarder une trajectoire de 200 ns avec un logiciel de visualisation appelé VMD. Les molécules d’eau ont été retirées pour faciliter la visualisation.

1.	Ouvrir VMD
2.	Charger la trajectoire : File --> new molecule

<img width="380" height="159" alt="image" src="https://github.com/user-attachments/assets/99f95b46-5543-4c18-9a60-3d5844e5bb5b" />

3.	Seules les liaisons des atomes apparaissent.
4.	
<img width="205" height="199" alt="image" src="https://github.com/user-attachments/assets/cd69b02a-79ac-40f3-bb59-3d489b44432a" />

On peut modifier la représentation : Graphics --> representation

<img width="236" height="119" alt="image" src="https://github.com/user-attachments/assets/67961147-4474-4aa4-92d0-66b4050d0dbc" />

Sélectionner « nucleic » ; Drawing method  « new ribbon » ; coloring methods « Resname », qui permet de colorer en fonction des bases nucléiques :
Adenine : rose		Thymine : blanc
Guanine : vert		Cytosine : vert clair	
Autres couleurs : bases nucléiques aux extrémités.

<img width="334" height="260" alt="image" src="https://github.com/user-attachments/assets/1a961114-3708-48d5-8d79-1b43b16c32c3" />

Créer une nouvelle représentation
Sélectionner « resname HTX » ; Drawing method « CPK » : chaque atome est représenté par une boule (cyan = carbone, bleu = azote, rouge = oxygène, blanc=hydrogène).

<img width="454" height="320" alt="image" src="https://github.com/user-attachments/assets/2175d852-806f-4fa6-b09b-6ffb72e8221a" />

Pour faciliter les observations, on peut faire les modifications suivantes dans Display : choisir Orthographic, enlever le depth Cueing.

4.	Observer la trajectoire et regarder ce qui se passe.

<img width="370" height="146" alt="image" src="https://github.com/user-attachments/assets/0f275180-ab5c-4e9a-b190-ccf7b820a2d1" />

-	D’où partent les molécules ? 
-	Vont-elles interagir avec l’ADN ? Si oui, où ? Au bout de combien de temps de simulation ? Les interactions durent elles « longtemps » ?
-	Les interactions ont-elles un impact sur la structure de l’ADN ?
