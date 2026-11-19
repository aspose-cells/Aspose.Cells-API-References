---
title: "PivotCache"
second_title: "Aspose.Cells for Java API 参考"
description: "表示某些数据透视表报告的内存缓存。"
type: docs
url: /zh/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

表示某些数据透视表报告的内存缓存。

**Remarks**

所有数据将被收集到此缓存中，数据透视表仅从此缓存获取数据，而不直接访问数据源。如果某些 [PivotTable](../../com.aspose.cells/pivottable)s 的数据源相同，它们将使用同一个数据透视缓存。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [dispose()](#dispose--) | 释放所有资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | 获取在丢弃未使用项之前允许的未使用项数量。 |
| [getPivotTables()](#getPivotTables--) | 获取使用此数据透视缓存的所有数据透视表。 |
| [getSourceType()](#getSourceType--) | 获取 [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype)。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | 从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表计算视图数据。 |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | 从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表计算视图数据。 |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | 设置在丢弃未使用项之前允许的未使用项数量。 |
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


释放所有资源。

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


获取在丢弃未使用项之前允许的未使用项数量。该值必须大于 -2 且小于 1048577。 [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst)；

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


获取使用此数据透视缓存的所有数据透视表。

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


获取 [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype)。

参见 [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype)。

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


从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表计算视图数据。

**Remarks**

如果 table1 和 table2 都使用此缓存，则两个表将被计算。最好直接调用 [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) 来刷新文件中的所有数据透视表和图表。

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表计算视图数据。

**Remarks**

最好直接调用 [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) 来刷新文件中的所有数据透视表和图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | 刷新数据透视表数据源的选项。 |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


设置在丢弃未使用项之前允许的未使用项数量。该值必须大于 -2 且小于 1048577。 [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst)；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

