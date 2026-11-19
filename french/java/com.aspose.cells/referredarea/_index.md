---
title: "ReferredArea"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une zone référencée par la formule."
type: docs
url: /fr/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

Représente une zone référencée par la formule.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | La colonne de fin de la zone. |
| [getEndRow()](#getEndRow--) | La ligne de fin de la zone. |
| [getExternalFileName()](#getExternalFileName--) | Obtient le nom du fichier externe si c’est une référence externe. |
| [getSheetName()](#getSheetName--) | Indique la feuille dans laquelle se trouve cette référence. |
| [getSheetNames()](#getSheetNames--) | Noms de toutes les feuilles de calcul auxquelles cette instance fait référence. |
| [getStartColumn()](#getStartColumn--) | La colonne de départ de la zone. |
| [getStartRow()](#getStartRow--) | La ligne de départ de la zone. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [getValues()](#getValues--) | Obtient les valeurs des cellules dans cette zone. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | Obtient les valeurs des cellules dans cette zone. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indique si c’est une zone. |
| [isEntireColumn()](#isEntireColumn--) | Indique si cette zone contient toutes les lignes (colonne entière). |
| [isEntireRow()](#isEntireRow--) | Indique si cette zone contient toutes les colonnes (ligne entière). |
| [isExternalLink()](#isExternalLink--) | Indique si c'est un lien externe. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Renvoie l'adresse de référence de cette zone. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


La colonne de fin de la zone.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


La ligne de fin de la zone.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Obtient le nom du fichier externe si c’est une référence externe.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Indique la feuille dans laquelle se trouve cette référence.

**Remarks**

Si elle fait référence à plusieurs feuilles de calcul, la valeur renvoyée est similaire à l'expression de plage dans la formule. Par exemple \"Sheet1:Sheet3\" pour la référence dans la formule \"=SUM(Sheet1:Sheet3!$A$1:$B$2)\".

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


Noms de toutes les feuilles de calcul auxquelles cette instance fait référence.

**Returns:**
java.lang.String[]
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


La colonne de départ de la zone.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


La ligne de départ de la zone.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | décalage de ligne depuis la ligne de départ de cette zone |
| colOffset | int | décalage de colonne depuis la ligne de départ de cette zone |

**Returns:**
java.lang.Object - \"\\#REF!\" si cette zone est invalide ; \"\\#N/A\" si le décalage donné est hors de cette zone ; sinon renvoie la valeur de la cellule à la position donnée.
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | décalage de ligne depuis la ligne de départ de cette zone |
| colOffset | int | décalage de colonne depuis la ligne de départ de cette zone |
| calculateFormulas | boolean | Indique s'il faut le calculer de manière récursive si la référence spécifiée est une formule |

**Returns:**
java.lang.Object - \"\\#REF!\" si cette zone est invalide ; \"\\#N/A\" si le décalage donné est hors de cette zone ; sinon renvoie la valeur de la cellule à la position donnée.
### getValues() {#getValues--}
```
public Object getValues()
```


Obtient les valeurs des cellules dans cette zone.

**Returns:**
java.lang.Object - Si cette zone est invalide, \"\\#REF!\" sera renvoyé ; si cette zone est une seule cellule, alors renvoie l'objet valeur de la cellule ; sinon renvoie un tableau 2D contenant toutes les valeurs de cette zone.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


Obtient les valeurs des cellules dans cette zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calculateFormulas | boolean | Dans cette plage, s'il existe des formules qui n'ont pas été calculées, ce drapeau indique si ces formules doivent être calculées de manière récursive |

**Returns:**
java.lang.Object - Si cette zone est invalide, \"\\#REF!\" sera renvoyé ; si cette zone est une seule cellule, alors renvoie l'objet valeur de la cellule ; sinon renvoie un tableau 2D contenant toutes les valeurs de cette zone.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Indique si c’est une zone.

**Remarks**

Si ce n'est pas une zone, seuls StartRow et StartColumn ont effet.

**Returns:**
boolean
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


Indique si cette zone contient toutes les lignes (colonne entière).

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


Indique si cette zone contient toutes les colonnes (ligne entière).

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Indique si c'est un lien externe.

**Returns:**
boolean
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


Renvoie l'adresse de référence de cette zone. En général, il s'agit de l'adresse de la référence qui peut être utilisée dans une formule, comme \"Sheet1!A1:C3\".

**Returns:**
java.lang.String - l'adresse de référence de cette zone.
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

