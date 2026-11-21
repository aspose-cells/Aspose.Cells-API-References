---
title: "ExternalLinkCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la colección de enlaces externos en un libro de trabajo."
type: docs
url: /es/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Representa la colección de enlaces externos en un libro de trabajo.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Agregar un enlace externo. |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Agrega un enlace externo. |
| [clear()](#clear--) | Elimina todos los enlaces externos. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Elimina todos los enlaces externos. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [ExternalLink](../../com.aspose.cells/externallink) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos realmente contenidos en la colección. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtén un enumerador que recorra esta colección. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el enlace externo especificado del libro de trabajo. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Elimina el enlace externo especificado del libro de trabajo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Agregar un enlace externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). El tipo de directorio del nombre de archivo. |
| fileName | java.lang.String | el nombre de archivo. |
| sheetNames | java.lang.String[] | Todos los nombres de hoja del archivo externo. |

**Returns:**
int - La posición del nombre externo en esta lista.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Agrega un enlace externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo externo. |
| sheetNames | java.lang.String[] | Todos los nombres de hoja del archivo externo. |

**Returns:**
int - La posición del nombre externo en esta lista.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los enlaces externos.

**Remarks**

Al eliminar enlaces externos, todas las fórmulas que hacen referencia a ellos también se eliminarán porque las referencias se vuelven inválidas.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Elimina todos los enlaces externos.

**Remarks**

Si se requiere actualizar las referencias, esas referencias de enlaces externos en las fórmulas se cambiarán al libro de trabajo actual cuando sea posible. Por ejemplo, la fórmula original de una celda es "='externalsource.xlam'!customfunction()", después de eliminar los enlaces externos, la fórmula se convertirá en "=customfunction()"; Cuando la fórmula original es "='[externalsource.xlam]Sheet1'!$A$1", según si existe una hoja con el nombre "Sheet1" en el libro de trabajo actual: si es verdadero, la fórmula se convertirá en "=Sheet1!$A$1"; si es falso, la fórmula se convertirá en "=\#REF!$A$1".

Si no se requiere actualizar las referencias, todas las fórmulas con referencias a enlaces externos también se eliminarán porque esas referencias se vuelven inválidas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Indica si se actualizan todas las referencias de enlaces externos en las fórmulas a referencias del propio libro de trabajo actual. |

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
public ExternalLink get(int index)
```


Obtiene el elemento [ExternalLink](../../com.aspose.cells/externallink) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
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


Obtiene el número de elementos realmente contenidos en la colección.

**Returns:**
int
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


Obtén un enumerador que recorra esta colección.

**Returns:**
java.util.Iterator -
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


Elimina el enlace externo especificado del libro de trabajo.

**Remarks**

Al eliminar el enlace externo, todas las fórmulas que hacen referencia a él también se eliminarán porque las referencias se vuelven inválidas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del enlace externo que se eliminará. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Elimina el enlace externo especificado del libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del enlace externo que se eliminará. |
| updateReferencesAsLocal | boolean | Indica si se actualizan todas las referencias del enlace externo dado a la referencia del propio libro de trabajo actual. Consulte [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) para obtener más detalles sobre este parámetro. |

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

