---
title: "ReserveMissingPivotItemType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa cómo mantener los elementos de tabla dinámica faltantes."
type: docs
url: /es/java/com.aspose.cells/reservemissingpivotitemtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReserveMissingPivotItemType
```

Representa cómo mantener los elementos de tabla dinámica faltantes.
## Campos

| Campo | Descripción |
| --- | --- |
| [ALL](#ALL) | Reserva todos los elementos faltantes. |
| [DEFAULT](#DEFAULT) | Elimina los elementos de pivote faltantes antiguos y reserva los elementos eliminados de la nueva fuente de datos como elementos faltantes. |
| [NONE](#NONE) | Elimina todos los elementos de pivote faltantes. |
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
### ALL {#ALL}
```
public static final int ALL
```


Reserva todos los elementos faltantes.

**Remarks**

En Excel, mientras Excel no se cierre, los elementos faltantes generados desde la primera actualización de la tabla dinámica se conservarán, incluso si se actualiza repetidamente

### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```


Elimina los elementos de pivote faltantes antiguos y reserva los elementos eliminados de la nueva fuente de datos como elementos faltantes.

### NONE {#NONE}
```
public static final int NONE
```


Elimina todos los elementos de pivote faltantes.

**Remarks**

Se ignorará el orden de los elementos de pivote antiguos que faltan.

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

