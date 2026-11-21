---
title: "GridRow"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una sola imagen en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Encapsula el objeto que representa una sola imagen en una hoja de cálculo.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Obtiene la celda. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Obtenga la celda por índice específico en la lista. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Obtiene la primera celda de la fila. |
| [getHeight()](#getHeight--) | Obtiene la altura de la fila en unidades de puntos. |
| [getHidden()](#getHidden--) | Indica si la fila está oculta. |
| [getIndex()](#getIndex--) | Obtiene el índice de esta fila. |
| [getLastCell()](#getLastCell--) | Obtiene la última celda de la fila. |
| [getLastDataCell()](#getLastDataCell--) | Obtiene la última celda de la fila. |
| [getOutlineLevel()](#getOutlineLevel--) | Obtiene el nivel de esquema. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indica si la fila contiene algún dato |
| [iterator()](#iterator--) | Obtiene el enumerador de celdas |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Establece la altura de la fila en unidades de puntos. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica si la fila está oculta. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Establece el nivel de esquema. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Obtiene la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Obtenga la celda por índice específico en la lista.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Row.GetEnumerator() para iterar todas las celdas de esta fila. Esta propiedad será eliminada 12 meses después desde febrero de 2015. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición. |

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


Obtiene la primera celda de la fila.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtiene la altura de la fila en unidades de puntos.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Indica si la fila está oculta.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de esta fila.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Obtiene la última celda de la fila.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Obtiene la última celda de la fila.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Obtiene el nivel de esquema.

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


Indica si la fila contiene algún dato

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de celdas

**Returns:**
java.util.Iterator - El enumerador de celdas
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


Establece la altura de la fila en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica si la fila está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Establece el nivel de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte |  |

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

