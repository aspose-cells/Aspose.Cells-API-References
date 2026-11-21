---
title: "SheetSet"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Describe un conjunto de hojas."
type: docs
url: /es/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Describe un conjunto de hojas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Crea un conjunto de hojas basado en índices de hoja exactos. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Crea un conjunto de hojas basado en nombres de hoja exactos. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Obtiene un conjunto con la hoja activa del libro. |
| [getAll()](#getAll--) | Obtiene un conjunto con todas las hojas del libro en su orden original. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Obtiene un conjunto con las hojas visibles del libro en su orden original. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Crea un conjunto de hojas basado en índices de hoja exactos.

**Remarks**

Si se encuentra una hoja que no está en el libro, se lanzará una excepción durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndexes | int[] | índices de hoja basados en cero. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Crea un conjunto de hojas basado en nombres de hoja exactos.

**Remarks**

Si se encuentra una hoja que no está en el libro, se lanzará una excepción durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetNames | java.lang.String[] | nombres de hoja. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Obtiene un conjunto con la hoja activa del libro.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Obtiene un conjunto con todas las hojas del libro en su orden original.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Obtiene un conjunto con las hojas visibles del libro en su orden original.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

