---
title: "MultipleFilterCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la colección de filtros múltiples."
type: docs
url: /es/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Representa la colección de filtros múltiples.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Construye una nueva instancia. |
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Agrega un valor de criterio de filtro de fecha. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Agrega un valor de criterio de filtro de fecha y hora. |
| [add(String filter)](#add-java.lang.String-) | Agrega un criterio de filtro de etiqueta. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) o un valor de cadena. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el recuento de los valores de filtro. |
| [getMatchBlank()](#getMatchBlank--) | Indica si se debe filtrar por vacío. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtenga el enumerador para el valor de filtro, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Indica si se debe filtrar por vacío. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Construye una nueva instancia.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor establezca FilterColumn.FilterType como FilterType.MultipleFilters y luego obtenga FilterColumn.MultipleFilters. Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Agrega un valor de criterio de filtro de fecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). El tipo de filtro de fecha. |
| año | int | El año. |
| mes | int | El mes. |
| día | int | El día. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Agrega un valor de criterio de filtro de fecha y hora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). El tipo de filtro de fecha. |
| año | int | El año. |
| mes | int | El mes. |
| día | int | El día. |
| hora | int | La hora. |
| minuto | int | El minuto. |
| segundo | int | El segundo. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Agrega un criterio de filtro de etiqueta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filtro | java.lang.String | Los datos del filtro. |

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
public Object get(int index)
```


Obtiene [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) o un valor de cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
java.lang.Object - 
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


Obtiene el recuento de los valores de filtro.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Indica si se debe filtrar por vacío.

**Returns:**
boolean
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


Obtenga el enumerador para el valor de filtro,

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




### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Indica si se debe filtrar por vacío.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

