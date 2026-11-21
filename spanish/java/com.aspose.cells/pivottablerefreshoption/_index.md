---
title: "PivotTableRefreshOption"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de actualización de la fuente de datos de la tabla dinámica."
type: docs
url: /es/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

Representa las opciones de actualización de la fuente de datos de la tabla dinámica.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | Representa las opciones de actualización de la fuente de datos de la tabla dinámica. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Indica si se deben mantener los datos de grupo local en caché si los valores máximo y mínimo permanecen sin cambios. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Representa cómo reservar los elementos dinámicos faltantes. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Indica si se debe mantener el orden original de los elementos dinámicos como la fuente de datos anterior. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Indica si se deben mantener los datos de grupo local en caché si los valores máximo y mínimo permanecen sin cambios. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Indica si se debe mantener el orden original de los elementos dinámicos como la fuente de datos anterior. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Representa cómo reservar los elementos dinámicos faltantes. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


Representa las opciones de actualización de la fuente de datos de la tabla dinámica.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Indica si se deben mantener los datos de grupo local en caché si los valores máximo y mínimo permanecen sin cambios. El valor predeterminado es false, lo que significa actualizar el grupo con la configuración local.

**Remarks**

Esta es una solución temporal, por favor localice las tablas dinámicas implementando [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Representa cómo reservar los elementos dinámicos faltantes.

Vea [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


Indica si se debe mantener el orden original de los elementos dinámicos como la fuente de datos anterior.

**Remarks**

Solo aplicable al campo dinámico que no está ordenado. Al actualizar este tipo de campo dinámico, Ms Excel mantiene el orden original de la fuente de datos anterior. El valor predeterminado de esta propiedad es true, lo que representa el mismo comportamiento que Ms Excel. Si el usuario necesita que el campo dinámico se actualice completamente como los datos en la nueva fuente de datos, esta propiedad debe establecerse como false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


Indica si se deben mantener los datos de grupo local en caché si los valores máximo y mínimo permanecen sin cambios. El valor predeterminado es false, lo que significa actualizar el grupo con la configuración local.

**Remarks**

Esta es una solución temporal, por favor localice las tablas dinámicas implementando [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Indica si se debe mantener el orden original de los elementos dinámicos como la fuente de datos anterior.

**Remarks**

Solo aplicable al campo dinámico que no está ordenado. Al actualizar este tipo de campo dinámico, Ms Excel mantiene el orden original de la fuente de datos anterior. El valor predeterminado de esta propiedad es true, lo que representa el mismo comportamiento que Ms Excel. Si el usuario necesita que el campo dinámico se actualice completamente como los datos en la nueva fuente de datos, esta propiedad debe establecerse como false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Representa cómo reservar los elementos dinámicos faltantes.

Vea [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

