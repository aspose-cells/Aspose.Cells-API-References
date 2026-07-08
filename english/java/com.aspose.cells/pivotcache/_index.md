---
title: PivotCache
second_title: Aspose.Cells for Java API Reference
description: Represents the memory cache for some PivotTable reports.
type: docs
url: /java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Represents the memory cache for some PivotTable reports.

**Remarks**

All data will be gathered into this cache,and the pivot table only get data from this cache,not directly access data source. If data source of some [PivotTable](../../com.aspose.cells/pivottable)s are same, they will use a pivot cache.
## Constructors

| Constructor | Description |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Methods

| Method | Description |
| --- | --- |
| [dispose()](#dispose--) | Release all resource. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPivotTables()](#getPivotTables--) | Gets all pivot tables with this pivot cache. |
| [getSourceType()](#getSourceType--) | Gets the [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
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


Release all resource.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Gets all pivot tables with this pivot cache.

**Returns:**
com.aspose.cells.PivotTable[] - 
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Gets the [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

See [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

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


Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

**Remarks**

If both table1 and table2 use this cache, the two table will calculated. It's better that you can simply call [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) to refresh all pivot tables and charts in the file.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

**Remarks**

It's better that you can simply call [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) to refresh all pivot tables and charts in the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | The options for refreshing data source of pivot table. |

**Returns:**
int
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

