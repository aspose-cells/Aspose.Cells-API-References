---
title: "ValidationCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la colección de validación de datos."
type: docs
url: /es/java/com.aspose.cells/validationcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ValidationCollection extends CollectionBase
```

Representa la colección de validación de datos.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         Validation validation = validations.get(validations.add(area));
         validation.setType(com.aspose.cells.ValidationType.LIST);
         validation.setFormula1("a,b,c,d");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add()](#add--) | Añade una validación de datos a la colección. |
| [add(CellArea ca)](#add-com.aspose.cells.CellArea-) | Añade una validación de datos a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [Validation](../../com.aspose.cells/validation) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Obtiene la validación aplicada a la celda dada. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Elimina todas las configuraciones de validación en la celda. |
| [removeArea(CellArea ca)](#removeArea-com.aspose.cells.CellArea-) | Elimina todas las configuraciones de validación en el rango.. |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Añade una validación de datos a la colección.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método ValidationCollection.Add(CellArea). Este método será eliminado 12 meses después desde ENERO de 2015. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int - índice del objeto [Validation](../../com.aspose.cells/validation).
### add(CellArea ca) {#add-com.aspose.cells.CellArea-}
```
public int add(CellArea ca)
```


Añade una validación de datos a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El área contiene esta validación. |

**Returns:**
int - índice del objeto [Validation](../../com.aspose.cells/validation).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los objetos de la instancia de CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
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
public Validation get(int index)
```


Obtiene el elemento [Validation](../../com.aspose.cells/validation) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[Validation](../../com.aspose.cells/validation) - The element at the specified index.
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


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public Validation getValidationInCell(int row, int column)
```


Obtiene la validación aplicada a la celda dada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
[Validation](../../com.aspose.cells/validation) - Returns a [Validation](../../com.aspose.cells/validation) object or null if there is no validation for given cell
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Elimina todas las configuraciones de validación en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila de la celda. |
| columna | int | El índice de columna de la celda. |

### removeArea(CellArea ca) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea ca)
```


Elimina todas las configuraciones de validación en el rango..

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango que contiene la configuración de validaciones. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a eliminar. |

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

