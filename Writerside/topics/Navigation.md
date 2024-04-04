# Navigation

> Pour Naviguer dans les pages de l'appareil, cliquez sur les icones et bouttons grâce à l'écran tactile.
<note> Pour revenir en arrière, glissez votre doigt dans n'importe quelle direction.</note>

## Structure des pages

<code-block lang="mermaid">
graph TD
   A[Accueil]
   A --> B[Files]
   A --> C[Record]
   A --> D[Config]
    C --> E[Gesture List]
    C --> F[Record cycle]
D --> G[Time setting]
</code-block>

## Description des pages
<tabs>
<tab title="Accueil">
<img src="Main_screen.png" alt="main screen view" width="500"/>
<note>
<p>La page d'accueil est la première page affichée lors de l'allumage de l'appareil. Elle permet de naviguer vers les différentes fonctionnalités de l'appareil.</p>
<p>Les boutons "File", "Record" et "Config" permettent de naviguer vers les pages correspondantes.</p>
</note>
</tab>
<tab title="Files">
<img src="File_screen.png" alt="file screen view" width="500"/>
<note>
<p>La page "File" permet de visualiser les enregistrements effectués par l'appareil sur la carte micro SD. Elle affiche la liste des enregistrements avec le nom du geste, la date et l'heure de l'enregistrement.</p>
<p>Si une carte micro SD est insérée, les informations de la carte tels que le type et l'espace disponible sont affichées en haut de l'écran.</p>
<p>Si aucune carte micro SD n'est insérée, un message apparaît pour indiquer qu'aucune carte n'est détectée.</p>
</note> 
</tab>
<tab title="Record">
<img src="Record_screen.png" alt="record screen view" width="500"/>
<note>
<p>L'icone "Recorde cycle" permet d'acceder à la page homonyme.</p>
</note>
<note>
<p>L'icone "Manual Record" permet de lancer un enregistrement manuel du geste selectionné préalablement sur la page "Record list", par défaut le geste "CUSTOM" est selectionné.</p>
</note>
<note>
<p>l'icone "Record list" permet de selectionner le geste à enregistrer en accedant à la page "Record list".</p>
</note>
</tab>
<tab title="Config">
<img src="Config_screen.png" alt="config screen view" width="500"/>
<note>
<p>La page "Config" permet de visualiser l'état de l'appareil en indiquant par un icone rouge ou vert si la fonctionnalité est en fonction ou non.</p>
</note>
<note>
<p>En appuyant sur les icones, il est possible d'avoir plus d'information sur la fonctionnalité et d'obtenir de l'aide si besoin.</p>
</note>
<note>
<p>L'icone "Time" permet d'acceder à la page de configuration de l'heure "Time setting".</p>
</note>
</tab>
<tab title="Gesture List">
<img src="Gesture_List_screen.png" alt="gesture screen view" width="500"/>
<note>
<p>La page "Gesture List" permet de selectionner le geste à enregistrer parmis une liste modifiable dans le code (voir structure du projet). Par défaut le geste "CUSTOM" est selectionné.</p>
</note>
</tab>
<tab title="Record cycle">
<img src="Gesture_rep_screen.png" alt="record cycle screen view" width="500"/>  
<note>
<p>La page "Record cycle" permet de lancer un enregistrement automatique par appuis sur "Start".</p>
</note>
</tab>
<tab title="Time setting">
<img src="time_setting.png" alt="time setting screen view" width="500"/>
<note>
<p>La page "Time setting" permet de configurer l'heure de l'appareil. Elle affiche l'heure actuelle et permet de la modifier en appuyant sur les flèches "haut" ou "bas".</p>
</note>
<warning>
<p>Pour appliquer les modifications, il est nécessaire d'appuyer sur le bouton "reset" situé sous l'appareil.</p>
</warning>
</tab>
</tabs>