---
title: "PivotPageFields"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los elementos de página pivote si la fuente de datos de la tabla dinámica son rangos de consolidación."
type: docs
url: /es/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Representa los elementos de página pivote si la fuente de datos de la tabla dinámica son rangos de consolidación. Sólo puede contener hasta 4 elementos.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Representa los elementos de campo de página pivote. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Establece qué etiqueta de elemento en cada campo de página usar para identificar el rango de datos. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Añade un campo de página. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Obtiene el número de campos de página. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Representa los elementos de campo de página pivote.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Establece qué etiqueta de elemento en cada campo de página usar para identificar el rango de datos. pageItemIndex.Length debe ser igual a PageFieldCount, así que por favor añada primero el campo de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeIndex | int | El índice del rango de datos de consolidación. |
| pageItemIndex | int[] | El índice del elemento de página en cada campo de página. pageItemIndex[2] = 1 significa que el segundo elemento en el tercer campo se usa para identificar este rango. pageItemIndex[1] = -1 significa que no hay elemento en el segundo campo para identificar este rango y MS creará automáticamente un elemento \"blank\" en el segundo campo para identificar este rango. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Añade un campo de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageItems | java.lang.String[] | Etiqueta del elemento de campo de página |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Obtiene el número de campos de página.

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

