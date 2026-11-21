---
title: "TxtValueQuoteType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica el tipo de uso de comillas para los valores en archivos de formato de texto."
type: docs
url: /es/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

Especifica el tipo de uso de comillas para los valores en archivos de formato de texto.
## Campos

| Campo | Descripción |
| --- | --- |
| [ALWAYS](#ALWAYS) | Todos los valores siempre estarán entre comillas. |
| [MINIMUM](#MINIMUM) | Solo ponga comillas a los valores cuando sea necesario. |
| [NEVER](#NEVER) | Todos los valores no estarán entre comillas. |
| [NORMAL](#NORMAL) | Todos los valores que contengan caracteres especiales como comillas, carácter separador, estarán entre comillas. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Todos los valores siempre estarán entre comillas.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


Solo ponga comillas a los valores cuando sea necesario. Por ejemplo, si un valor contiene una comilla pero la comilla no está al principio de este valor, ese valor no será entre comillas.

### NEVER {#NEVER}
```
public static final int NEVER
```


Todos los valores no estarán entre comillas. El archivo de texto exportado con este tipo puede no leerse correctamente porque faltan las comillas necesarias.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Todos los valores que contengan caracteres especiales como comillas, carácter separador, estarán entre comillas. Lo mismo ocurre con el comportamiento de MS Excel al exportar archivos de texto.

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

