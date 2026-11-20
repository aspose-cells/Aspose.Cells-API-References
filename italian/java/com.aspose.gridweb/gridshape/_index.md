---
title: "GridShape"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un oggetto forma."
type: docs
url: /it/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Rappresenta un oggetto forma.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Ottiene il buffer dell'oggetto. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Ottiene l'ID del set per la forma. |
| [getLeft()](#getLeft--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [getLeftToCorner()](#getLeftToCorner--) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Ottiene il tipo di disegno mso. |
| [getName()](#getName--) | Ottiene il nome della forma. |
| [getText()](#getText--) | Rappresenta la stringa in questo oggetto TextBox. |
| [getTop()](#getTop--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [getTopToCorner()](#getTopToCorner--) | Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Rappresenta l'indice di riga dell'angolo in alto a sinistra. |
| [getZOrderPosition()](#getZOrderPosition--) | Restituisce la posizione di una forma nell'ordine Z. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Crea l'immagine e la salva in uno stream nel formato png specificato. |
| [setID(String value)](#setID-java.lang.String-) | Ottiene l'ID del set per la forma. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [setText(String value)](#setText-java.lang.String-) | Rappresenta la stringa in questo oggetto TextBox. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Restituisce la posizione di una forma nell'ordine Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Ottiene il buffer dell'oggetto.

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


Ottiene l'ID del set per la forma.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Ottiene il tipo di disegno mso.

Vedi [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome della forma.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Rappresenta la stringa in questo oggetto TextBox.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel.

**Remarks**

Se la forma è nel grafico, rappresenta lo spostamento verticale della forma dal suo bordo superiore.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Rappresenta l'indice della colonna dell'angolo superiore sinistro.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Rappresenta l'indice di riga dell'angolo in alto a sinistra.

**Remarks**

Se la forma è nella forma o nel gruppo, UpperLeftRow verrà ignorato.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Restituisce la posizione di una forma nell'ordine Z.

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


Crea l'immagine e la salva in uno stream nel formato png specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Ottiene l'ID del set per la forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Rappresenta la stringa in questo oggetto TextBox.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Restituisce la posizione di una forma nell'ordine Z.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

