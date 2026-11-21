---
title: "GridNameCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Encapsula una colección de objetos [GridName](../../com.aspose.gridweb/gridname).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Define un nuevo nombre en la hoja especificada. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Define un nuevo nombre global. |
| [clear()](#clear--) | Elimina todos los Nombres; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [GridName](../../com.aspose.gridweb/gridname) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el tamaño del enumerador |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtiene el enumerador de filas |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Elimina una matriz de nombres. |
| [removeAt(int index)](#removeAt-int-) | Elimina el nombre en el índice específico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Define un nuevo nombre en la hoja especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | El índice de hoja en el que se aplica el nombre. |
| texto | java.lang.String | Texto del nombre. No puede tener nombre de hoja. |
| refersTo | java.lang.String | La fórmula a la que se define el nombre. Debe tener nombre de hoja. p.ej. 'hoja hola!'A1:B2. |

**Returns:**
int - índice del objeto Name.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Define un nuevo nombre global.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | Texto del nombre. Puede tener nombre de hoja. |
| refersTo | java.lang.String | La fórmula a la que se define el nombre. Debe tener un nombre de hoja. p.ej. 'hoja hola!'A1:B2. |

**Returns:**
int - índice del objeto Name.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los Nombres;

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
public GridName get(int index)
```


Obtiene el elemento [GridName](../../com.aspose.gridweb/gridname) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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


Obtiene el enumerador de filas

**Returns:**
java.util.Iterator - El enumerador de filas
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Elimina una matriz de nombres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| names | java.lang.String[] | El texto de los nombres. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el nombre en el índice específico.

**Remarks**

Asegúrese de que el nombre no sea referenciado por otras fórmulas antes de llamar al método. Y si el nombre está referenciado, establezca solo Name.RefersTo como null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

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

