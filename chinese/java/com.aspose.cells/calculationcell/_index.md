---
title: "CalculationCell"
second_title: "Aspose.Cells for Java API 参考"
description: "表示正在计算的单元格的相关计算数据。"
type: docs
url: /zh/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

表示正在计算的单元格的相关计算数据。

**Remarks**

在公式计算过程中，用户不应更改工作簿中的任何数据，否则可能导致意外结果或异常。因此，此类提供的所有对象（例如 [getCell()](../../com.aspose.cells/calculationcell\#getCell--) 的 Cell 对象）仅用于“读取”目的。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | 获取正在计算的 Cell 对象。 |
| [getCellColumn()](#getCellColumn--) | 获取单元格的列索引。 |
| [getCellRow()](#getCellRow--) | 获取单元格的行索引。 |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | 获取 Workbook 对象。 |
| [getWorksheet()](#getWorksheet--) | 获取单元格所在的 Worksheet 对象。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | 设置单元格的计算值。 |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


获取正在计算的 Cell 对象。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


获取单元格的列索引。

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


获取单元格的行索引。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取 Workbook 对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取单元格所在的 Worksheet 对象。

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


设置单元格的计算值。

**Remarks**

用户可以通过此方法设置计算结果，以忽略对该单元格的自动计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| v | java.lang.Object |  |

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

