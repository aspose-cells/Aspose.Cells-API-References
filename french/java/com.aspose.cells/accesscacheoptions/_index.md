---
title: "AccessCacheOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options de mise en cache pour l'accès aux données."
type: docs
url: /fr/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Options de mise en cache pour l'accès aux données. Plusieurs options peuvent être combinées à l'aide de l'opérateur "\|".

**Remarks**

Pour certaines fonctionnalités, l'accès à un grand jeu de données nécessite de nombreuses opérations répétées et complexes telles que la recherche, le calcul, etc., et ces opérations prennent beaucoup de temps supplémentaire. Dans les situations courantes, toutes les données dépendantes restent inchangées pendant l'accès, de sorte que certains caches peuvent être créés et utilisés pour améliorer les performances d'accès. À cette fin, nous fournissons cette API afin que l'utilisateur puisse spécifier quel type d'accès aux données doit être optimisé par un mécanisme de mise en cache éventuel.

Veuillez noter que, selon les options, différents ensembles de données peuvent devoir être en lecture seule. Et la performance de l'accès aux données dépend de nombreux aspects ; l'utilisation d'un mécanisme de mise en cache ne garantit pas une amélioration des performances. Dans certaines situations, comme lorsque le jeu de données à accéder est petit, l'utilisation du cache peut même prendre plus de temps, car la mise en cache elle-même nécessite également un certain temps supplémentaire.
## Champs

| Champ | Description |
| --- | --- |
| [ALL](#ALL) | Applique toutes les optimisations possibles pour tous les types d'accès aux données dans le classeur. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Applique une optimisation possible pour le calcul des formules. |
| [CELLS_DATA](#CELLS-DATA) | Applique une optimisation possible pour l'obtention des valeurs des cellules. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Applique une optimisation possible pour obtenir les résultats liés à l'affichage des cellules([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Applique une optimisation possible pour obtenir le résultat de formatage des mises en forme conditionnelles. |
| [GET_FORMULA](#GET-FORMULA) | Applique une optimisation possible pour obtenir les formules. |
| [NONE](#NONE) | Pas de cache pour aucun accès aux données. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Applique une optimisation possible pour obtenir la position et la taille de l'objet (tel que Shape). |
| [SET_FORMULA](#SET-FORMULA) | Applique une optimisation possible pour définir les formules. |
| [VALIDATION](#VALIDATION) | Applique une optimisation possible pour obtenir le résultat de validation. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Applique toutes les optimisations possibles pour tous les types d'accès aux données dans le classeur. Tous les paramètres et données ne doivent pas être modifiés pendant l'accès optimisé.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Applique une optimisation possible pour le calcul des formules. Les données des cellules ne doivent pas être modifiées pendant l'accès optimisé, aucun nouvel objet (Cell, Row, etc.) ne doit être créé non plus (par exemple via [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Applique une optimisation possible pour l'obtention des valeurs des cellules. Les données des cellules (données et paramètres de Cell, Row) ne doivent pas être modifiées pendant l'accès optimisé, aucun nouvel objet Cell/Row ne doit être créé non plus (par exemple via [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Applique une optimisation possible pour obtenir les résultats liés à l'affichage des cellules(...). Les données des cellules et les objets liés au style (styles Cell/Row/Column, largeur de colonne, etc.) ne doivent pas être modifiés pendant l'accès optimisé.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Appliquer une optimisation possible pour obtenir le résultat de mise en forme des formats conditionnels. Toutes les données et paramètres pouvant affecter le résultat des formats conditionnels (paramètres des formats conditionnels, valeurs des cellules dépendantes, etc.) ne doivent pas être modifiés pendant l'accès optimisé.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Appliquer une optimisation possible pour obtenir les formules. Toutes les données et paramètres pouvant affecter l'expression de la formule (nom de la feuille de calcul, texte du nom, colonne du tableau, etc.) ne doivent pas être modifiés pendant l'accès optimisé.

### NONE {#NONE}
```
public static final int NONE
```


Pas de cache pour aucun accès aux données.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Appliquer une optimisation possible pour obtenir la position et la taille d'un objet (tel qu'une forme). Les paramètres de hauteur de ligne et de largeur de colonne ne doivent pas être modifiés pendant l'accès optimisé.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Appliquer une optimisation possible pour définir les formules. Toutes les données et paramètres pouvant affecter l'expression de la formule (nom de la feuille de calcul, texte du nom, colonne du tableau, etc.) ne doivent pas être modifiés pendant l'accès optimisé.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Appliquer une optimisation possible pour obtenir le résultat de validation. Toutes les données et paramètres pouvant affecter le résultat de la validation (paramètres de la validation, valeurs des cellules dépendantes, etc.) ne doivent pas être modifiés pendant l'accès optimisé.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

