---
title: "SessionMode"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el modo de sesión de la cuadrícula."
type: docs
url: /es/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

Representa el modo de sesión de la cuadrícula.
## Campos

| Campo | Descripción |
| --- | --- |
| [CUSTOM](#CUSTOM) | Utiliza el evento LoadCustomData para cargar los datos de la hoja del grid manualmente. |
| [FILE](#FILE) | Utiliza el archivo del sistema para almacenar/recuperar los datos de la hoja del grid automáticamente, el usuario necesita establecer SessionStorePath para especificar el directorio del archivo. |
| [SESSION](#SESSION) | Utiliza la sesión del sistema para almacenar/recuperar los datos de la hoja del grid automáticamente. |
| [VIEW_STATE](#VIEW-STATE) | Utiliza el viewstate de la página para almacenar/recuperar los datos de la hoja del grid automáticamente. |
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
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Utiliza el evento LoadCustomData para cargar los datos de la hoja del grid manualmente. Y utiliza el evento SheetDataUpdated para guardar los datos de la hoja del grid.

### FILE {#FILE}
```
public static final int FILE
```


Utiliza el archivo del sistema para almacenar/recuperar los datos de la hoja del grid automáticamente, el usuario necesita establecer SessionStorePath para especificar el directorio del archivo.

### SESSION {#SESSION}
```
public static final int SESSION
```


Utiliza la sesión del sistema para almacenar/recuperar los datos de la hoja del grid automáticamente.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


Utiliza el viewstate de la página para almacenar/recuperar los datos de la hoja del grid automáticamente.

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

