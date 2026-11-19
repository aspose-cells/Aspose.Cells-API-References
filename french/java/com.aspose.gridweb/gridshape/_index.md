---
title: "GridShape"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un objet forme."
type: docs
url: /fr/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Représente un objet forme.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Obtient le tampon de l'objet. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Obtient le Sets ID pour la Shape. |
| [getLeft()](#getLeft--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [getLeftToCorner()](#getLeftToCorner--) | Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Obtient le type de dessin mso. |
| [getName()](#getName--) | Obtient le nom de la forme. |
| [getText()](#getText--) | Représente la chaîne dans cet objet TextBox. |
| [getTop()](#getTop--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels. |
| [getTopToCorner()](#getTopToCorner--) | Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Représente l’indice de colonne du coin supérieur gauche. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Représente l'index de ligne du coin supérieur gauche. |
| [getZOrderPosition()](#getZOrderPosition--) | Renvoie la position d'une forme dans l'ordre Z. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Crée l'image et l'enregistre dans un flux au format png spécifié. |
| [setID(String value)](#setID-java.lang.String-) | Obtient le Sets ID pour la Shape. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels. |
| [setText(String value)](#setText-java.lang.String-) | Représente la chaîne dans cet objet TextBox. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Renvoie la position d'une forme dans l'ordre Z. |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Obtient le tampon de l'objet.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```


Obtient le Sets ID pour la Shape.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Obtient le type de dessin mso.

Voir [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la forme.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Représente la chaîne dans cet objet TextBox.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels.

**Remarks**

Si la forme se trouve dans le graphique, représente le décalage vertical de la forme par rapport à sa bordure supérieure.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Représente l’indice de colonne du coin supérieur gauche.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Représente l'index de ligne du coin supérieur gauche.

**Remarks**

Si la forme est dans une forme ou dans un groupe, UpperLeftRow sera ignoré.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Renvoie la position d'une forme dans l'ordre Z.

**Returns:**
int
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




### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Crée l'image et l'enregistre dans un flux au format png spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Obtient le Sets ID pour la Shape.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Représente la chaîne dans cet objet TextBox.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Renvoie la position d'une forme dans l'ordre Z.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

