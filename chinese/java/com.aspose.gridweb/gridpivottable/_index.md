---
title: "GridPivotTable"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表上的 PivotTable 报表。"
type: docs
url: /zh/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

表示工作表上的数据透视表报告。PivotTable 对象是 [GridPivotTable](../../com.aspose.gridweb/gridpivottable) 集合的成员。PivotTables 集合包含控件上的所有 PivotTable 对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | 将字段添加到特定区域。 |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | 将字段添加到特定区域。 |
| [calculateData()](#calculateData--) | 计算数据透视表的数据到单元格。 |
| [clearAllFields()](#clearAllFields--) | 清除所有数据透视字段。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | 根据字段类型获取特定字段。 |
| [fields(String fieldName)](#fields-java.lang.String-) | 根据字段名称获取特定字段。 |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | 从其数据源刷新数据透视表的数据和设置。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


将字段添加到特定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype)。字段区域类型。 |
| baseFieldIndex | int | 基字段中的字段索引。 |

**Returns:**
int - 特定字段中的字段位置。
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


将字段添加到特定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype)。字段区域类型。 |
| fieldName | java.lang.String | 基字段中的名称。 |

**Returns:**
int - 特定字段中的字段位置。如果不存在相应名称的字段，返回 -1。
### calculateData() {#calculateData--}
```
public void calculateData()
```


计算数据透视表的数据到单元格。

**Remarks**

如果未调用该方法，枢轴范围内的 Cell.Value 可能无法返回正确结果。此方法使用内部枢轴缓存计算数据，而非原始数据源。因此如果数据源已更改，请先调用 RefreshData() 方法。

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


清除所有数据透视字段。

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


根据字段类型获取特定字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype)。字段类型。 |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


根据字段名称获取特定字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldName | java.lang.String | 字段名称。 |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


从其数据源刷新数据透视表的数据和设置。

**Remarks**

我们将从数据源收集数据到数据透视缓存，然后将缓存中的数据计算到单元格中。此方法仅用于将所有数据收集到数据透视缓存。

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

