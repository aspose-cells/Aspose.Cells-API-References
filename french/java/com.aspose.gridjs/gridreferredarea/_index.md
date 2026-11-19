---
title: "GridReferredArea"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une zone référencée par la formule."
type: docs
url: /fr/java/com.aspose.gridjs/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
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
| [getSheetName()](#getSheetName--) | Indique dans quelle feuille cela se trouve |
| [getStartColumn()](#getStartColumn--) | La colonne de départ de la zone. |
| [getStartRow()](#getStartRow--) | La ligne de départ de la zone. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [getValues()](#getValues--) | Obtient les valeurs des cellules dans cette zone. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indique si c’est une zone. |
| [isExternalLink()](#isExternalLink--) | Indique si c'est un lien externe. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
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


Indique dans quelle feuille cela se trouve

**Returns:**
java.lang.String
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
### getValues() {#getValues--}
```
public Object getValues()
```


Obtient les valeurs des cellules dans cette zone.

**Returns:**
java.lang.Object - Si cette zone est invalide, \"\\#REF!\" sera retourné ; Si cette zone ne comporte qu'une seule cellule, alors retourner l'objet valeur de la cellule ; Sinon retourner un tableau contenant toutes les valeurs de cette zone.
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

