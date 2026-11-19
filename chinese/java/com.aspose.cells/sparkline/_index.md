---
title: "迷你图"
second_title: "Aspose.Cells for Java API 参考"
description: "Sparkline 表示工作表单元格中的微型图表或图形，提供数据的可视化表示。"
type: docs
url: /zh/java/com.aspose.cells/sparkline/
---

**Inheritance:**
java.lang.Object
```
public class Sparkline
```

Sparkline 表示工作表单元格中的微型图表或图形，提供数据的可视化表示。

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, sheet.getName() + "!A1:D1", false, ca);
 
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         idx = group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         Sparkline line = group.getSparklines().get(idx);
         System.out.println("Saprkline data range: " + line.getDataRange() + ", row: " + line.getRow() + ", column: " + line.getColumn());
         line.toImage("output.png", new ImageOrPrintOptions());
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取迷你图的列索引. |
| [getDataRange()](#getDataRange--) | 表示迷你图的数据范围. |
| [getRow()](#getRow--) | 获取迷你图的行索引. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataRange(String value)](#setDataRange-java.lang.String-) | 表示迷你图的数据范围. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | 将迷你图转换为图像. |
| [toImage(String fileName, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | 将迷你图转换为图像. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


获取迷你图的列索引.

**Returns:**
int
### getDataRange() {#getDataRange--}
```
public String getDataRange()
```


表示迷你图的数据范围.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


获取迷你图的行索引.

**Returns:**
int
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




### setDataRange(String value) {#setDataRange-java.lang.String-}
```
public void setDataRange(String value)
```


表示迷你图的数据范围.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


将迷你图转换为图像.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 图像流. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | 图像选项. |

### toImage(String fileName, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String fileName, ImageOrPrintOptions options)
```


将迷你图转换为图像.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 图像文件名. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | 图像选项 |

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

