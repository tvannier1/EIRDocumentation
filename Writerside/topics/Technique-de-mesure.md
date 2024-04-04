# Technique de mesure

La mesure de l'impédance électrique des tissus est une étape cruciale dans la réalisation d'une tomographie d'impédance électrique. Elle permet de caractériser les propriétés électriques des tissus et de générer des images de leur distribution.

## Principe de fonctionnement
L'EIT repose sur la mesure des variations d'impédance électrique des tissus en réponse à un courant alternatif. Cette méthode non invasive permet de cartographier la distribution de l'impédance électrique à l'intérieur d'un objet ou d'un corps.

Dans ce projet, l'impédance électrique est mesurée à l'aide d'un circuit intégré [AD5933](https://www.analog.com/media/en/technical-documentation/data-sheets/ad5933.pdf) qui génère un signal sinusoïdal à une fréquence donnée. Ce signal est appliqué aux 8 électrodes de mesure qui sont en contact avec les tissus. L'impédance électrique est ensuite calculée à partir de la tension et du courant mesurés.


<img src="carto.png" alt="Cartographie de l'impédance électrique"/>

Ainsi, une tomographie d'impédance électrique permet de visualiser la distribution de l'impédance électrique des tissus.

Pour selectionner les deux électrodes de mesure, on utilise des multiplexeurs analogiques [TMUX4051](https://www.ti.com/lit/ds/symlink/tmux4051.pdf?ts=1712103773180). Ces composants permettent de commuter les électrodes de mesure en fonction de la configuration souhaitée.

Enfin, un [MCP23008](https://ww1.microchip.com/downloads/en/DeviceDoc/21919e.pdf)  permet de configurer les broches de sortie et de les activer/désactiver en fonction des besoins. Dans ce projet, le MCP23008 est utilisé comme une interface entre le microcontrôleur et les composants de mesure notamment grace au protocole I2C.

### Synoptique du système

```mermaid
    graph LR
        A[AD5933]
        B[TMUX4051]
        F[TMUX4051]
        C[MCP23008]
        D[M5Stack Core S3]
        E[Electrodes]

D --- C
C --- A
A --- B
A --- F
B --- E
F --- E
```





