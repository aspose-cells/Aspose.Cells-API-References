---
title: "GridRow"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une image unique dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Encapsule l'objet qui représente une image unique dans une feuille de calcul.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Obtient la cellule. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Obtenez la cellule par un indice spécifique dans la liste. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Obtient la première cellule de la ligne. |
| [getHeight()](#getHeight--) | Obtient la hauteur de la ligne en points. |
| [getHidden()](#getHidden--) | Indique si la ligne est masquée. |
| [getIndex()](#getIndex--) | Obtient l'index de cette ligne. |
| [getLastCell()](#getLastCell--) | Obtient la dernière cellule de la ligne. |
| [getLastDataCell()](#getLastDataCell--) | Obtient la dernière cellule de la ligne. |
| [getOutlineLevel()](#getOutlineLevel--) | Obtient le niveau de contour. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indique si la ligne contient des données |
| [iterator()](#iterator--) | Obtient l'énumérateur de cellules |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Définit la hauteur de la ligne en points. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indique si la ligne est masquée. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Définit le niveau de contour. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Obtient la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Obtenez la cellule par un indice spécifique dans la liste.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Au lieu de cela, veuillez utiliser la méthode Row.GetEnumerator() pour parcourir toutes les cellules de cette ligne. Cette propriété sera supprimée 12 mois plus tard, depuis février 2015. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | La position. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Obtient la première cellule de la ligne.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtient la hauteur de la ligne en points.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Indique si la ligne est masquée.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de cette ligne.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Obtient la dernière cellule de la ligne.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Obtient la dernière cellule de la ligne.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Obtient le niveau de contour.

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indique si la ligne contient des données

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient l'énumérateur de cellules

**Returns:**
java.util.Iterator - L'énumérateur de cellules
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Définit la hauteur de la ligne en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indique si la ligne est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Définit le niveau de contour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte |  |

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

