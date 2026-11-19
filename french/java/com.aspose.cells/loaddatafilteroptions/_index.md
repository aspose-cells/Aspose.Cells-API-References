---
title: "LoadDataFilterOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de filtrage des données lors du chargement du classeur à partir d'un modèle."
type: docs
url: /fr/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Représente les options de filtrage des données lors du chargement du classeur à partir d'un modèle.
## Champs

| Champ | Description |
| --- | --- |
| [ALL](#ALL) | Charger tout |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Charger les paramètres du classeur |
| [CELL_BLANK](#CELL-BLANK) | Charger les cellules dont la valeur est vide |
| [CELL_BOOL](#CELL-BOOL) | Charger les cellules dont la valeur est booléenne |
| [CELL_DATA](#CELL-DATA) | Charger les données des cellules, y compris les valeurs, les formules et le formatage |
| [CELL_ERROR](#CELL-ERROR) | Charger les cellules dont la valeur est une erreur |
| [CELL_NUMERIC](#CELL-NUMERIC) | Charger les cellules dont la valeur est numérique (y compris la date/heure) |
| [CELL_STRING](#CELL-STRING) | Charger les cellules dont la valeur est une chaîne |
| [CELL_VALUE](#CELL-VALUE) | Charger uniquement la valeur des cellules (tous les types de valeurs) uniquement |
| [CHART](#CHART) | Charger les graphiques |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Charger le formatage conditionnel |
| [DATA_VALIDATION](#DATA-VALIDATION) | Charger les validations de données |
| [DEFINED_NAMES](#DEFINED-NAMES) | Charger les objets de nom définis |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Charger les propriétés du document |
| [DRAWING](#DRAWING) | Objets de dessin (y compris Chart, Picture, OleObject et tous les autres objets de dessin) |
| [FORMULA](#FORMULA) | Charger les formules de cellules. |
| [HYPERLINKS](#HYPERLINKS) | Charger les hyperliens |
| [MERGED_AREA](#MERGED-AREA) | Charger les cellules fusionnées |
| [NONE](#NONE) | Ne charger aucune donnée pour la feuille |
| [OLE_OBJECT](#OLE-OBJECT) | Charger les OleObjects |
| [PICTURE](#PICTURE) | Charger les images |
| [PIVOT_TABLE](#PIVOT-TABLE) | Charger les tableaux croisés dynamiques |
| [REVISION](#REVISION) | Charger les journaux de révision |
| [SETTINGS](#SETTINGS) | Charger les paramètres du classeur et de la feuille de calcul |
| [SHAPE](#SHAPE) | Charger les formes |
| [SHEET_DATA](#SHEET-DATA) | Charger toutes les données de la feuille de calcul, telles que les données des cellules, les paramètres, les objets, ...etc. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Charger les paramètres de la feuille de calcul |
| [STRUCTURE](#STRUCTURE) | Charger la structure du classeur |
| [STYLE](#STYLE) | Charger les styles de formatage des cellules |
| [TABLE](#TABLE) | Charger les tables |
| [VBA](#VBA) | Charger les projets VBA |
| [XML_MAP](#XML-MAP) | Charger XmlMap |
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


Charger tout

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Charger les paramètres du classeur

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Charger les cellules dont la valeur est vide

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Charger les cellules dont la valeur est booléenne

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Charger les données des cellules, y compris les valeurs, les formules et le formatage

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Charger les cellules dont la valeur est une erreur

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Charger les cellules dont la valeur est numérique (y compris la date/heure)

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Charger les cellules dont la valeur est une chaîne

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Charger uniquement la valeur des cellules (tous les types de valeurs) uniquement

### CHART {#CHART}
```
public static final int CHART
```


Charger les graphiques

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Charger le formatage conditionnel

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Charger les validations de données

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Charger les objets de nom définis

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Charger les propriétés du document

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Objets de dessin (y compris Chart, Picture, OleObject et tous les autres objets de dessin)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Charger les formules de cellules.

**Remarks**

Les objets Name généralement définis (DefinedNames) doivent également être chargés lors du chargement des formules car ils peuvent être référencés par les formules. Ainsi, l'option Formula ou CellData doit fonctionner avec l'option DefinedNames ensemble (Formula\|DefinedNames ou CellData\|DefinedNames) pour la plupart des scénarios.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Charger les hyperliens

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Charger les cellules fusionnées

### NONE {#NONE}
```
public static final int NONE
```


Ne charger aucune donnée pour la feuille

**Remarks**

NOTE : Ce membre est maintenant obsolète et veuillez utiliser Structure à la place. Cette propriété sera supprimée 12 mois plus tard à compter de décembre 2017. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


Charger les OleObjects

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Charger les images

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Charger les tableaux croisés dynamiques

### REVISION {#REVISION}
```
public static final int REVISION
```


Charger les journaux de révision

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Charger les paramètres du classeur et de la feuille de calcul

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Charger les formes

**Remarks**

NOTE : Ce membre est maintenant obsolète et veuillez utiliser Drawing à la place. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2019. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Charger toutes les données de la feuille de calcul, telles que les données des cellules, les paramètres, les objets, ...etc.

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Charger les paramètres de la feuille de calcul

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Charger la structure du classeur

### STYLE {#STYLE}
```
public static final int STYLE
```


Charger les styles de formatage des cellules

### TABLE {#TABLE}
```
public static final int TABLE
```


Charger les tables

### VBA {#VBA}
```
public static final int VBA
```


Charger les projets VBA

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


Charger XmlMap

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

