---
title: "RenameStrategy"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opción de estrategia para nombres duplicados de columnas."
type: docs
url: /es/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Opción de estrategia para nombres duplicados de columnas.

**Remarks**

Al procesar datos con encabezados, algunos escenarios requieren que los encabezados no se dupliquen en todas las columnas. Por ejemplo, al exportar datos a una datatable y que el encabezado deba tomarse como el nombre de columna de la datatable, los valores duplicados del encabezado son inválidos. Para este tipo de situaciones, el usuario puede determinar cómo manejarlos especificando esta estrategia.
## Campos

| Campo | Descripción |
| --- | --- |
| [DIGIT](#DIGIT) | Nombrado con dígito. |
| [EXCEPTION](#EXCEPTION) | Lanza una excepción. |
| [LETTER](#LETTER) | Nombrado con letra.. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Nombrado con dígito. Los nombres duplicados se convertirán en ...1, ...2, etc.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


Lanza una excepción.

### LETTER {#LETTER}
```
public static final int LETTER
```


Nombrado con letra.. Los nombres duplicados se convertirán en ...A, ...B, etc.

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

