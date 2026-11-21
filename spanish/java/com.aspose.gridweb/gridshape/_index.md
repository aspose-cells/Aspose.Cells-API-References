---
title: "GridShape"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un objeto de forma."
type: docs
url: /es/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Representa un objeto de forma.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Obtiene el Buffer del objeto. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Obtiene el Sets ID para la Shape. |
| [getLeft()](#getLeft--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles. |
| [getLeftToCorner()](#getLeftToCorner--) | Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Obtiene el tipo de dibujo mso. |
| [getName()](#getName--) | Obtiene el nombre de la forma. |
| [getText()](#getText--) | Representa la cadena en este objeto TextBox. |
| [getTop()](#getTop--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles. |
| [getTopToCorner()](#getTopToCorner--) | Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Representa el índice de columna de la esquina superior izquierda. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Representa el índice de fila de la esquina superior izquierda. |
| [getZOrderPosition()](#getZOrderPosition--) | Devuelve la posición de una forma en el orden Z. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Crea la imagen y la guarda en un flujo en el formato png especificado. |
| [setID(String value)](#setID-java.lang.String-) | Obtiene el Sets ID para la Shape. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles. |
| [setText(String value)](#setText-java.lang.String-) | Representa la cadena en este objeto TextBox. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Devuelve la posición de una forma en el orden Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Obtiene el Buffer del objeto.

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


Obtiene el Sets ID para la Shape.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Obtiene el tipo de dibujo mso.

Ver [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la forma.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Representa la cadena en este objeto TextBox.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles.

**Remarks**

Si la forma está en el gráfico, representa el desplazamiento vertical de la forma desde su borde superior.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Representa el índice de columna de la esquina superior izquierda.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Representa el índice de fila de la esquina superior izquierda.

**Remarks**

Si la forma está dentro de otra forma o en el grupo, UpperLeftRow será ignorado.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Devuelve la posición de una forma en el orden Z.

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


Crea la imagen y la guarda en un flujo en el formato png especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Obtiene el Sets ID para la Shape.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Representa la cadena en este objeto TextBox.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Devuelve la posición de una forma en el orden Z.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

