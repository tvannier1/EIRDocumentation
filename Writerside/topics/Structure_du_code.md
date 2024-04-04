# Structure du code


## Structure des fichiers

Le projet est structuré de la manière suivante :

<code-block lang="mermaid">
    graph LR
        A[main.cpp]
        B[EIT_Shared_Values.h]
        C[EIT_Impedance_measurement.cpp]
        D[EIT_Impedance_measurement.h]
        E[EIT_Interface_Display.cpp]
        F[EIT_Interface_Display.h]
        
        B --> A
        B --> F
        B --> D
        D --> A
        F --> A
        F --> E
        D --> E
        D --> C

</code-block>

## Description des fichiers
<tabs>
<tab title="main.cpp">
<p>Le fichier main.cpp est le point d'entrée du programme. Il contient la fonction setup() qui est appelée une seule fois au démarrage de l'appareil et la fonction loop() qui est appelée en boucle.</p>
<p>La fonction setup() initialise les différents composants de l'appareil et configure les paramètres de base. La fonction loop() gère l'interface utilisateur.</p>
</tab>
<tab title="EIT_Shared_Values.h">
<p>Le fichier EIT_Shared_Values.h contient les valeurs partagées entre les différents fichiers du projet. Il définit les constantes utilisées pour les calculs et les affichages.</p>
</tab>
<tab title="EIT_Impedance_measurement.cpp">
<p>Le fichier EIT_Impedance_measurement.cpp contient les fonctions permettant de mesurer l'impédance électrique des tissus. Il utilise la bibliothèque AD5933 pour effectuer les mesures.</p>
</tab>
<tab title="EIT_Impedance_measurement.h">
<p>Le fichier EIT_Impedance_measurement.h contient les déclarations des fonctions du fichier EIT_Impedance_measurement.cpp. Il permet d'inclure les fonctions dans d'autres fichiers du projet.</p>
</tab>
<tab title="EIT_Interface_Display.cpp">
<p>Le fichier EIT_Interface_Display.cpp contient les fonctions permettant d'afficher les informations à l'écran. Il utilise la bibliothèque M5Stack pour gérer l'affichage.</p>
</tab>
<tab title="EIT_Interface_Display.h">
<p>Le fichier EIT_Interface_Display.h contient les déclarations des fonctions du fichier EIT_Interface_Display.cpp. Il permet d'inclure les fonctions dans d'autres fichiers du projet.</p>
</tab>
</tabs>