# Etude d'un conditionneur de capteur capacitif




## 1. Objectif 
On se propose  d’étudier un conditionneur de capteur capacitif à variation de  fréquence basé sur un montage oscillant qui permet de convertir la variation de la capacité du  capteur en une variation ∆f de la fréquence d’oscillation du circuit. 

## 2. Les conditionneurs des capteurs passifs 
Un capteur passif convertit la variation du mesurande en une variation d’impédance. On  associe donc toujours une source externe de tension ou de courant au capteur. Deux grands  principes de conditionneurs peuvent être employés : 
∙ Montage en pont : On récupère alors une tension proportionnelle au mesurande. ∙ Montage oscillant : La fréquence du signal de sortie est modulée par le mesurande. 
Cas d’un conditionneur des capteurs capacitifs en montage oscillant 
Si on insère un capteur capacitif dans un circuit en montage oscillant : Oscillateur astable  NE555, la variation d’impédance du capteur entraîne une variation ∆f de la fréquence  d’oscillation du circuit. La période des oscillations est directement reliée à la valeur de la  capacité du capteur. 
✔ Oscillateur NE555 : 
Le NE555 est un circuit intégré à 8 bornes, spécialement conçu pour générer un signal  rectangulaire. 

 ![image](https://user-images.githubusercontent.com/92098387/226175720-eeda2530-9d8e-4cbb-ab84-24fbfea9f561.png)

 
La configuration astable permet d'utiliser le NE555 comme oscillateur. Deux résistances et un  condensateur permettent de modifier la fréquence d'oscillations ainsi que le rapport cyclique. 
Dans cette configuration, présentée par la figure 2, la bascule est réinitialisée  automatiquement à chaque cycle générant un train d'impulsion perpétuelle. 

![image](https://user-images.githubusercontent.com/92098387/226175744-9e05b35a-e197-4862-937e-0d938ea60cbb.png)


Une oscillation complète est effectuée lorsque le condensateur se charge jusqu'à 2/3 de Vcc et  se décharge à 1/3 de Vcc. Lors de la charge, les résistances Ra et Rb sont en série avec le  condensateur, mais la décharge s'effectue à travers la résistance Rb seulement. C'est de cette  façon que le rapport cyclique peut être modifié. La fréquence d'oscillations f ainsi que le  rapport cyclique α suivent les relations suivantes : 
 


## 3. Manipulation 

Matériels utilisés : 
∙ Paquet de cigarette vide 
∙ Papier aluminium 
∙ Colle 
∙ Deux résistances : Ra=Rb=10KΩ 
∙ Un condensateur de capacité 100nF 
∙ Le circuit intégré NE555
∙ Alimentation stabilisée 
∙ oscilloscope  
Travail demandé 

### a. Etude de l’oscillateur astable NE555 


f0 = 1.44 / ( r0 +2 RB ) * C = 1.44 / ( 10000 + 20000 ) * 10-9 = 48 Khz 


### 1. Réaliser le montage de la figure2. 

![image](https://user-images.githubusercontent.com/92098387/226175991-dc82dd84-8692-461d-8f98-32f88425b0d2.png)



### 2. A l’aide d’un oscilloscope, visualiser la sortie et déterminer la fréquence générée par  l’oscillateur. 

![image](https://user-images.githubusercontent.com/92098387/226175977-c4499cb1-067a-4563-99e7-d0190ba25643.png)

![image](https://user-images.githubusercontent.com/92098387/226175965-2f7952e5-2674-48b4-9d9c-f46ee224e4ef.png)

### 3. Calculer la fréquence générée par l’oscillateur en fonction des éléments du montage, La  comparer avec la valeur mesurée. 

F pratique = 40.9 Khz 
F théorique = 48 Khz 
on sait que les valeurs du Ra et Rb et C sont pas bien eu le premier propriete ( on prend les valeurs en theorique sur le calcul .. )  .. donc ces valeurs changes ( on doit prend des mesures pratique maintenant )  et du coup ces différences dans les valeurs   imposent  une changement sur la fréquence du signal de sortie  





### b. Fabrication d’un capteur capacitif de pression artisanale  

Pour la fabrication d’un capteur capacitif en utilisant des matériaux de base, On suit les étapes  suivantes: 
∙ Couper deux plaques de papier aluminium de parts égales. 
∙ Coller les deux parts d'aluminium sur chaque face de la part d’un paquet de cigarette vide. ∙ Scotcher des fils électriques (préalablement dénudés) sur chacune des plaques d'aluminium  afin d’avoir deux électrodes de connexion des deux armatures. 

### 1. Calculer la valeur de la capacité du capteur à vide (sans déformation).

### c. Etude du conditionneur de capteur capacitif en montage oscillant 

On insère le capteur capacitif dans le montage : oscillateur astable NE555 en parallèle avec la  capacité C=100 nF. 

### 1. Mesurer la fréquence à la sortie du circuit, en déduire la valeur de la capacité du capteur.  La comparer avec la valeur théorique. 

c = E0 Er * S / D = 8.86.10-12 *(107*10 3 +46*10 3)/13*10 -3 = 3.335.10 -5 
F en Theorique = 1.44 / ( 30000 ) * ( 1.00000335  * 10 -9 )  = 47.83 Khz 
⇒ vu qu’on ajouter une petit valeur du capacite on voit pas une grand variation sur le Fréquence  

![image](https://user-images.githubusercontent.com/92098387/226175942-f8b8b0fa-52a3-4334-a10a-50654d526051.png)


### 2. Appliquer une contrainte sur les deux facettes, visualiser le signal à la sortie du circuit et  interpréter le résultat. 

on vu que lorsqu' on applique une force sur notre “ capture “ la fréquence est diminue 



### 3. Pour une contrainte donnée x1, mesurer la fréquence à la sortie du circuit et déterminer la  valeur de la capacité du capteur.  

F = 1.44 / ( ra +2 rb ) ( c + cc ) => c + cc = 1.44/ (ra + 2rb) F 
⇒ cc = (1.44/ ra + 2 rb ) F ) - c  = 3.32 * 10-15 f ⇒ ressemble à notre valeur théorique 

![image](https://user-images.githubusercontent.com/92098387/226175929-3a8660af-bed5-40f7-b9fa-09ddd3160dce.png)


On introduit du coton dans le paquet de cigarette vide. 

### 1. Mesurer la fréquence à la sortie du circuit.  
F = 50 Khz 

### 2. Déterminer la valeur de la capacité du capteur. Interpréter le résultat.
 
c = 1.001*10-15 F 

![image](https://user-images.githubusercontent.com/92098387/226175914-83f95e95-21dd-4806-afbf-b3fcd205dfa3.png)


L'ajout de coton dans le paquet va modifier la valeur de la capacité du capteur en réduisant la surface de contact entre les deux surfaces d'aluminium. Cela va entraîner une diminution de la capacité et donc une augmentation de la fréquence à la sortie du circuit
⇒ le coton agit comme un isolant électrique et réduit la surface de contact entre les deux plaques du capteur, ce qui diminue la capacité et augmente la fréquence à la sortie du circuit.


