---
title: "TipoMétodoReconexión"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión."
type: docs
url: /es/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión.
## Campos

| Campo | Descripción |
| --- | --- |
| [ALWAYS](#ALWAYS) | En cada actualización, obtener la información de conexión actualizada del archivo de conexión externo, si está disponible, y usarla en lugar de la información de conexión existente. |
| [NEVER](#NEVER) | Nunca obtener información de conexión actualizada del archivo de conexión externo, incluso si está disponible y aunque la información de conexión existente sea inválida. |
| [REQUIRED](#REQUIRED) | Al actualizar, usar la información de conexión existente y, si resulta ser inválida, obtener la información de conexión actualizada, si está disponible en el archivo de conexión externo. |
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


En cada actualización, obtener la información de conexión actualizada del archivo de conexión externo, si está disponible, y usarla en lugar de la información de conexión existente. En este caso, la actualización de datos fallará si el archivo de conexión externo no está disponible.

### NEVER {#NEVER}
```
public static final int NEVER
```


Nunca obtener información de conexión actualizada del archivo de conexión externo, incluso si está disponible y aunque la información de conexión existente sea inválida.

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


Al actualizar, usar la información de conexión existente y, si resulta ser inválida, obtener la información de conexión actualizada, si está disponible en el archivo de conexión externo.

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

