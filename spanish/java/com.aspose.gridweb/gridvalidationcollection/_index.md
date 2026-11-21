---
title: "GridValidationCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Encapsula una colección de objetos [GridValidation](../../com.aspose.gridweb/gridvalidation).
## Métodos

| Método | Descripción |
| --- | --- |
| [add()](#add--) | Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Añade una validación de datos a la colección. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección. |
| [add(int row, int column)](#add-int-int-) | Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección. La validación se aplica a la celda especificada. |
| [add(String cellname)](#add-java.lang.String-) | Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección. La validación se aplica a la celda especificada. |
| [clear()](#clear--) | Borra todas las validaciones. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [GridValidation](../../com.aspose.gridweb/gridvalidation) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el tamaño del enumerador |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Obtiene la validación aplicada a la celda dada. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina la validación en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método GridValidationCollection.Add(fila,columna). Esta propiedad será eliminada 12 meses después desde ENERO 2015. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Añade una validación de datos a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El área contiene esta validación. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Un objeto de validación. |

**Returns:**
int - índice del objeto [GridValidation](../../com.aspose.gridweb/gridvalidation).
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección. La validación se aplica a la celda especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Agrega un [GridValidation](../../com.aspose.gridweb/gridvalidation) a la colección. La validación se aplica a la celda especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellname | java.lang.String | el nombre de la celda. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Borra todas las validaciones.

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
### get(int index) {#get-int-}
```
public GridValidation get(int index)
```


Obtiene el elemento [GridValidation](../../com.aspose.gridweb/gridvalidation) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
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


Obtiene el tamaño del enumerador

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Obtiene la validación aplicada a la celda dada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina la validación en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

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

