---
title: "QueryTable"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 QueryTable 信息。"
type: docs
url: /zh/java/com.aspose.cells/querytable/
---

**Inheritance:**
java.lang.Object
```
public class QueryTable
```

表示 QueryTable 信息。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Getting the first query table in the worksheet if exists
         //QueryTable qt = worksheet.QueryTables[0];
         //Getting display address of the query table.
         //string address = qt.ResultRange.Address;
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--) | 返回或设置对象的 AdjustColumnWidth。 |
| [getClass()](#getClass--) |  |
| [getConnectionId()](#getConnectionId--) | 获取查询表的连接 ID。 |
| [getExternalConnection()](#getExternalConnection--) | 获取关联的外部连接。 |
| [getName()](#getName--) | 获取查询表的名称。 |
| [getPreserveFormatting()](#getPreserveFormatting--) | 返回或设置对象的 PreserveFormatting。 |
| [getResultRange()](#getResultRange--) | 获取结果的范围。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdjustColumnWidth(boolean value)](#setAdjustColumnWidth-boolean-) | 返回或设置对象的 AdjustColumnWidth。 |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | 返回或设置对象的 PreserveFormatting。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```
public boolean getAdjustColumnWidth()
```


返回或设置对象的 AdjustColumnWidth。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


获取查询表的连接 ID。

**Returns:**
int
### getExternalConnection() {#getExternalConnection--}
```
public ExternalConnection getExternalConnection()
```


获取关联的外部连接。

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getName() {#getName--}
```
public String getName()
```


获取查询表的名称。

**Returns:**
java.lang.String
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


返回或设置对象的 PreserveFormatting。

**Returns:**
boolean
### getResultRange() {#getResultRange--}
```
public Range getResultRange()
```


获取结果的范围。

**Returns:**
[Range](../../com.aspose.cells/range) - 
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




### setAdjustColumnWidth(boolean value) {#setAdjustColumnWidth-boolean-}
```
public void setAdjustColumnWidth(boolean value)
```


返回或设置对象的 AdjustColumnWidth。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


返回或设置对象的 PreserveFormatting。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

