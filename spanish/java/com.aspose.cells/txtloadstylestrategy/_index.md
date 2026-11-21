---
title: "TxtLoadStyleStrategy"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica cómo aplicar estilo a los valores analizados al convertir una cadena a número o fecha/hora."
type: docs
url: /es/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Especifica cómo aplicar estilo a los valores analizados al convertir una cadena a número o fecha/hora.
## Campos

| Campo | Descripción |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Establezca el estilo como número/fecha y hora incorporado cuando el valor analizado sea un valor numérico/fecha y hora simple. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Establezca el formato personalizado exacto para el valor analizado para que el valor formateado sea idéntico al valor de entrada original. |
| [NONE](#NONE) | No establece estilo para el valor analizado. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Establezca el estilo como número/fecha y hora incorporado cuando el valor analizado sea un valor numérico/fecha y hora simple.

**Remarks**

Cuando MS Excel analiza valores de fecha y hora o numéricos según la entrada del usuario (como un archivo CSV), el formato de esos valores puede cambiar, por ejemplo, ceros iniciales/finales del número, el orden año/mes/día de la fecha y hora, etc. Este tipo sirve para simular el comportamiento de MS Excel.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Establezca el formato personalizado exacto para el valor analizado para que el valor formateado sea idéntico al valor de entrada original.

### NONE {#NONE}
```
public static final int NONE
```


No establece estilo para el valor analizado.

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

