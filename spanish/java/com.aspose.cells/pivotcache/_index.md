---
title: "PivotCache"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la caché de memoria para algunos informes de tabla dinámica."
type: docs
url: /es/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Representa la caché de memoria para algunos informes de tabla dinámica.

**Remarks**

Todos los datos se recopilarán en esta caché, y la tabla dinámica solo obtendrá datos de esta caché, sin acceder directamente a la fuente de datos. Si la fuente de datos de algunas [PivotTable](../../com.aspose.cells/pivottable)s es la misma, usarán una caché de tabla dinámica.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [dispose()](#dispose--) | Liberar todos los recursos. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Obtiene el número de elementos no utilizados que se permiten antes de descartar los elementos no utilizados. |
| [getPivotTables()](#getPivotTables--) | Obtiene todas las tablas dinámicas con esta caché de tabla dinámica. |
| [getSourceType()](#getSourceType--) | Obtiene el [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Establece el número de elementos no utilizados que se permiten antes de descartar los elementos no utilizados. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


Liberar todos los recursos.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Obtiene el número de elementos no utilizados que se permiten antes de descartar los elementos no utilizados. Este valor DEBE ser mayor que -2 y menor que 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Obtiene todas las tablas dinámicas con esta caché de tabla dinámica.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Obtiene el [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

Ver [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
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




### refresh() {#refresh--}
```
public int refresh()
```


Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica.

**Remarks**

Si tanto table1 como table2 usan esta caché, ambas tablas se calcularán. Es mejor que simplemente llames a [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) para actualizar todas las tablas dinámicas y gráficos en el archivo.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica.

**Remarks**

Es mejor que simplemente llames a [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) para actualizar todas las tablas dinámicas y gráficos en el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Las opciones para actualizar la fuente de datos de la tabla dinámica. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Establece el número de elementos no utilizados que se permiten antes de descartar los elementos no utilizados. Este valor DEBE ser mayor que -2 y menor que 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

