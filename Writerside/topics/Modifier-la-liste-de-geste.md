# Modifier la liste de geste

Pour modifier la liste des gestes, il suffit de modifier le tableau `gesture_list` dans le fichier `EIT_Shared_Values.h`(voir [Structure du code](Structure_du_code.md)) .
\
\
Ce tableau contient la liste des gestes disponibles pour l'enregistrement. Chaque geste est représenté par une chaîne de caractères.

```cpp
// Gesture list
const String gestureList[] = {"CUSTOM",
                              "FIST",
                              "INDEX_PINCH", 
                              "LEFT", 
                              "RELAX", 
                              "RIGHT", 
                              "STRETCH", 
                              "THUMB_UP"
                              // Add your gesture here
                              };
```
