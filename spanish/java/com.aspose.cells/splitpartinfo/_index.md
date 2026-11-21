---
title: "SplitPartInfo"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la información de una entrada/salida para múltiples entradas/salidas, como la página actual que se renderizará al convertir la hoja de cálculo a imagen."
type: docs
url: /es/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Representa la información de una entrada/salida para múltiples entradas/salidas, como la página actual que se renderiza al convertir una hoja de cálculo a imagen.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Índice de la parte actual en la secuencia (basado en 0) |
| [getSheetIndex()](#getSheetIndex--) | Índice de la hoja donde se encuentra la parte actual. -1 indica que solo hay una hoja. |
| [getSheetName()](#getSheetName--) | Nombre de la hoja donde se encuentra la parte actual. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Índice de la parte actual en la secuencia (basado en 0). -1 significa que no hay múltiples partes, por lo que el resultado es único.

**Remarks**

Si se necesitan procesar varias hojas y cada hoja se procesa(separada) por separado, el índice de parte siempre comienza en 0 para cada hoja. Por ejemplo, al convertir el libro de trabajo a imágenes, representa el índice de página de salida de la hoja que se está procesando actualmente. Y -1 indica que solo hay una página para la hoja actual.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Índice de la hoja donde se encuentra la parte actual. -1 indica que solo hay una hoja.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Nombre de la hoja donde se encuentra la parte actual.

**Remarks**

Puede ser nulo en algunas situaciones, como al renderizar todo el libro de trabajo a una imagen TIFF.

**Returns:**
java.lang.String
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

