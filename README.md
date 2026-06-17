# Simulation de l’interaction entre 4 molécules HTX et l’ADN

<em>Nota Bene : pour une meilleure lisibilité, les images de ce tutoriel peuvent être agrandies en cliquant dessus.</em>

## Étude de structures moléculaires avec Avogadro

Avogadro est un outil très intéressant pour visualiser la structure des molécules. Pour commencer, nous allons dessiner une molécule.

1. Cliquer sur « Search » et taper Avogadro.

<img width="731" height="752" alt="Screenshot 2026-06-17 at 13 52 28" src="https://github.com/user-attachments/assets/ab226e99-140d-4e66-9572-954f1e40be68" />

2. Sélectionner l'outil de dessin et le type d'élément (par exemple le carbone).

<img width="961" height="669" alt="Screenshot 2026-06-17 at 13 53 15" src="https://github.com/user-attachments/assets/0427d34a-8fa7-4b30-a4fd-f1965d7a0abf" />

3. Appuyer sur l’écran pour créer un atome.

<img width="860" height="671" alt="Screenshot 2026-06-17 at 13 54 44" src="https://github.com/user-attachments/assets/611ddb88-a3f4-48c9-81fe-919c4abe77ed" />

4. Pour ajouter un autre atome, cliquer sur un atome existant puis faire glisser la souris.

<img width="958" height="713" alt="Screenshot 2026-06-17 at 13 55 35" src="https://github.com/user-attachments/assets/e9fe3a9c-2be5-4a78-8584-876dacdc6490" />

5. Il est possible d'utiliser des liaisons doubles ou triples en changeant l’ordre de liaison. Attention, si la case “Adjust Hydrogens” est cochée, l'atome créé sera lié automatiquement à des hydrogènes.

<img width="1052" height="777" alt="Screenshot 2026-06-17 at 13 57 52" src="https://github.com/user-attachments/assets/3729b6d8-5a94-4b13-a7e0-e00a3a6d7585" />

6. Il existe plusieurs outils qui peuvent aider à mieux visualiser la molécule.

<img width="714" height="326" alt="Screenshot 2026-06-17 at 13 58 51" src="https://github.com/user-attachments/assets/e4fc071a-5327-4844-8a03-b23378c813a5" />

7. Avogadro possède aussi un outil très utile pour « optimiser » les molécules. Cela signifie qu’il corrige automatiquement la structure (distances, angles) pour obtenir une forme plus stable, comme dans la réalité. Pour commencer on va changer la méthode d’optimisation. Cliquer sur « Extensions », puis « Calculate » et « Configure ». Choisir GAFF comme Force Field. Puis « OK ».

<img width="995" height="626" alt="Screenshot 2026-06-17 at 14 00 05" src="https://github.com/user-attachments/assets/ff1e1124-ae1f-420e-a020-9f40a408ec64" />

8. Cliquer sur « Extensions » puis « Optimize Geometry ». Observer comment la molécule se réorganise toute seule pour retrouver sa forme la plus stable.

Maintenant que nous savons utiliser les outils de base d’Avogadro, nous allons dessiner quelques molécules, par exemple les structures suivantes :

<img width="1130" height="335" alt="Screenshot 2026-06-17 at 14 01 35" src="https://github.com/user-attachments/assets/a57b4c6c-9718-4148-a193-96d94a7d1f92" />

Maintenant que nous savons comment créer une molécule, nous allons ouvrir un fichier provenant d’un calcul déjà effectué.  Cela nous permettra d’observer la structure la plus stable de la molécule ainsi que ses orbitales, qui sont comme des “nuages” autour des atomes où se trouvent les électrons. Elles nous montrent où les électrons ont le plus de chances d’être.

9. Télécharger les fichiers `dp1953a.fchk` et `htx.fchk`, disponibles sur cette page GitHub.

10. Ouvrir un fichier `.fchk` en cliquant sur « File » puis « Open ».

11. Sélectionner une orbitale pour la visualiser.

<img width="1252" height="654" alt="Screenshot 2026-06-17 at 14 03 47" src="https://github.com/user-attachments/assets/6ed3e226-7ce4-4a9d-b36a-c113d3d76b61" />

## Visualisation d'une simulation avec VMD

<p align="justify">
Pour comprendre comment la molécule HTX interagit avec l’ADN, il est possible de simuler un fragment de deux brins d’ADN formant une double hélice et 4 molécules dans l’eau et observer comment les molécules interagissent.
</p>
<p align="justify">
Dans la méthode utilisée, les atomes sont des boules reliées par des ressorts qui représentent les liaisons chimiques fortes. Les interactions chimiques faibles sont reproduites grâce aux propriétés des boules. Cette approche, appelée méthode « classique », permet de simuler le comportement de plusieurs centaines de milliers d’atomes pour des durées allant de la dizaine de nanosecondes à quelques microsecondes.
</p>
<p align="justify">
Ici, on va regarder une trajectoire de 200 ns avec un logiciel de visualisation appelé VMD. Les molécules d’eau ont été retirées pour faciliter la visualisation.
</p>

### Tutoriel

1. Ouvrir le logiciel VMD à l'aide du terminal.

<img width="1913" height="1049" alt="Terminal1" src="https://github.com/user-attachments/assets/da50e704-8b1c-4d77-9a05-a86be6a5041c" />

<img width="1913" height="1049" alt="Terminal2" src="https://github.com/user-attachments/assets/39bb7a5b-d90e-4ad2-baec-a1f0d56dab1a" />

2.	Télécharger le dossier `center_dsDNA_4htx.zip` disponible sur cette page GitHub. Le décompresser pour obtenir le fichier contenant la trajectoire : `center_dsDNA_4htx.pdb`.

3.	Charger la trajectoire : `File` --> `New Molecule`

La fenêtre suivante s'ouvre. Sélectionner le fichier de trajectoire et le charger.

<img width="1199" height="605" alt="Screenshot 2026-06-11 at 15 14 36" src="https://github.com/user-attachments/assets/f49c5dac-8b53-4b7c-9344-b285b13aef92" />

4.	Seules les liaisons des atomes apparaissent.

<img width="1034" height="1056" alt="Screenshot 2026-06-11 at 15 20 06" src="https://github.com/user-attachments/assets/9f1e0447-e3db-487c-8d9d-a61dd72582ee" />

On peut modifier la représentation : `Graphics` --> `Representations`

<img width="562" height="359" alt="Screenshot 2026-06-11 at 15 35 27" src="https://github.com/user-attachments/assets/b803fb5a-efba-4252-8607-aa8dd5b0fe62" />

Sélectionner « nucleic » ; Drawing Method  « new ribbon » ; Coloring Method « Resname », qui permet de colorer en fonction des bases nucléiques :<br>
Adenine : rose<br>
Thymine : blanc<br>
Guanine : vert<br>
Cytosine : vert clair<br>
Autres couleurs : bases nucléiques aux extrémités.

<img width="1316" height="1022" alt="Screenshot 2026-06-11 at 15 28 54" src="https://github.com/user-attachments/assets/0db6ee45-c55c-461b-a179-e39a56483f51" />

Créer une nouvelle représentation :<br>
Sélectionner « resname HTX » ; Drawing Method « CPK » : chaque atome est représenté par une boule (cyan = carbone, bleu = azote, rouge = oxygène, blanc=hydrogène).

<img width="1108" height="873" alt="Screenshot 2026-06-11 at 15 33 23" src="https://github.com/user-attachments/assets/d9cd15ca-fdc8-4375-9de8-231e55d9a4a3" />

Pour faciliter les observations, on peut faire les modifications suivantes dans `Display` : choisir `Orthographic`, enlever le `Depth Cueing`.

5.	Observer la trajectoire et regarder ce qui se passe.

<img width="696" height="414" alt="Screenshot 2026-06-11 at 15 40 16" src="https://github.com/user-attachments/assets/7d64bb12-cabe-4b46-91ea-f5c2f7cd87ab" />

### Questions

-	D’où partent les molécules ? 
-	Vont-elles interagir avec l’ADN ? Si oui, où ? Au bout de combien de temps de simulation ? Les interactions durent elles « longtemps » ?
-	Les interactions ont-elles un impact sur la structure de l’ADN ?
