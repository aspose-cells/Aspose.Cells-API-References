---
title: "MemorySetting"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Modos de uso de memoria para el modelo de datos de celdas."
type: docs
url: /es/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Modos de uso de memoria para el modelo de datos de celdas.
## Campos

| Campo | Descripción |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Se prefiere el rendimiento de memoria y usar un archivo en lugar de memoria para mantener los datos de las celdas. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Se prefiere el rendimiento de memoria. |
| [NORMAL](#NORMAL) | Modo predeterminado para el modelo de celdas. |
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
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


Se prefiere el rendimiento de memoria y usar un archivo en lugar de memoria para mantener los datos de las celdas.

**Remarks**

Con este modo, los datos de las celdas se mantendrán en formato compacto y la mayor parte de los datos se mantendrá en un archivo temporal en lugar de en memoria. Por lo tanto, al comparar con el modo [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE), este modo puede reducir aún más el consumo de memoria, pero las operaciones de E/S para acceder a los datos de las celdas también generarán un mayor costo de tiempo.

Esta opción está disponible desde la versión v25.7.0.

| Algunos límites notables y operaciones recomendadas al usar este modo: |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Cuando se usa este modo para cualquier hoja de cálculo en un libro, se debe llamar a [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) al final del trabajo para liberar todos los recursos, como los archivos temporales. |
| Acceder a las celdas de forma aleatoria producirá un bajo rendimiento porque los datos deben leerse aleatoria y repetidamente (por lo que el puntero en el archivo se cambiará en consecuencia y se requerirán operaciones de E/S repetidas). Si es posible, acceda siempre a los datos de forma secuencial (fila por fila). |
| Cuando se modifica el dato de una fila/celda, los datos de otras celdas/filas también pueden verse afectados (por ejemplo, los datos pueden desplazarse/moverse a otros lugares para asignar suficiente espacio al dato modificado). Por lo tanto, cada cambio de cualquier dato requiere la sincronización de otros objetos existentes (como el objeto Row o Cell). Así, para obtener un mejor rendimiento, no mantenga varias Rows/Cells al mismo tiempo. Procesarlos uno por uno reducirá la sincronización de datos y mejorará el rendimiento. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Se prefiere el rendimiento de memoria.

**Remarks**

Con este modo, los datos de las celdas se mantendrán en formato compacto para reducir el consumo de memoria. Por otro lado, los datos compactos también pueden generar un mayor costo de tiempo, especialmente al actualizar los datos de las celdas o al acceder a ellos de forma aleatoria.

Esta opción está disponible desde la versión v8.0.0.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Modo predeterminado para el modelo de celdas.

**Remarks**

Este modo se aplica a todas las versiones.

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

