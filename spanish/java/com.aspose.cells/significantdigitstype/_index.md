---
title: "SignificantDigitsType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el tipo de dígitos significativos para la salida de valores numéricos."
type: docs
url: /es/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Representa el tipo de dígitos significativos para la salida de valores numéricos.
## Campos

| Campo | Descripción |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15-dígitos |
| [G_17](#G-17) | 17-dígitos al formatear el valor con "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17-dígitos al redondear el valor. |
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
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15-dígitos

### G_17 {#G-17}
```
public static final int G_17
```


17-dígitos al formatear el valor con "G17".

**Remarks**

Para algunos valores double, "G17" puede dar un valor diferente al original/literal ingresado por el usuario. Por ejemplo, el valor double 0.15 se mostrará como 0.14999999999999999; el valor double 1.0E-16 se mostrará como 9.9999999999999998E-17. Excel de Microsoft maneja esos valores de forma inconsistente, guarda 0.15 como 0.15 en el archivo xlsx, pero para 1.0E-16 el valor guardado en el archivo xlsx es 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17-dígitos al redondear el valor.

**Remarks**

Este tipo generalmente devuelve el valor tal como el original/literal ingresado por el usuario. Para 0.15 produce "0.15" y para 1.0E-16 produce "1.0E-16". Pero también existen algunos casos especiales que pueden dar valores diferentes al literal. Por ejemplo, al redondear 208435494.96478021 a 17-dígitos("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#"), la salida es 208435494.96478.

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

