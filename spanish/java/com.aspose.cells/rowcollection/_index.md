---
title: "RowCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Recopila los objetos que representan las filas individuales en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Recopila los objetos [Row](../../com.aspose.cells/row) que representan las filas individuales en una hoja de cálculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [clear()](#clear--) | Borrar todas las filas y celdas. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Obtiene un objeto [Row](../../com.aspose.cells/row) por el índice de fila dado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de filas en esta colección. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Obtiene el objeto fila por la posición en la lista. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtiene un enumerador que recorre las filas de esta colección |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Obtiene un enumerador que recorre las filas de esta colección |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento de fila en el índice (posición) especificado de esta colección. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Borrar todas las filas y celdas.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Obtiene un objeto [Row](../../com.aspose.cells/row) por el índice de fila dado. El objeto Row del índice de fila dado se instanciará si no existe previamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de filas en esta colección.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Obtiene el objeto fila por la posición en la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene un enumerador que recorre las filas de esta colección

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - El enumerador de filas que recorrerá todas las filas existentes en esta colección.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Obtiene un enumerador que recorre las filas de esta colección

**Remarks**

Si la colección de filas se modifica (por operaciones que pueden causar que se instancie una nueva Row o que se elimine una Row existente) durante el recorrido con el enumerador, se debe usar un enumerador sincronizado en lugar del enumerador normal para que el recorrido pueda continuar desde la posición justo después de la que fue recorrida por el último MoveNext(). Sin embargo, junto con la ventaja de que no se omita ni se recorra repetidamente ningún elemento, la desventaja del enumerador sincronizado es que el rendimiento se degradará un poco en comparación con el enumerador normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| revertido | boolean | si enumerar filas en orden invertido |
| sincronizar | boolean | si el enumerador devuelto debe comprobar la modificación de la colección de filas y mantenerse sincronizado con ella. |

**Returns:**
java.util.Iterator - El enumerador de filas que recorrerá todas las filas existentes en esta colección.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el elemento de fila en el índice (posición) especificado de esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | índice basado en cero (posición, no [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) del elemento de fila existente en esta colección. |

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

