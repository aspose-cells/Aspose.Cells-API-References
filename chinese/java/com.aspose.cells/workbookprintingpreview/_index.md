---
title: "WorkbookPrintingPreview"
second_title: "Aspose.Cells for Java API 参考"
description: "工作簿打印预览。"
type: docs
url: /zh/java/com.aspose.cells/workbookprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookPrintingPreview
```

工作簿打印预览。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)](#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | WorkbookPrintingPreview 的构造 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | 评估此工作簿的总页数 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options) {#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```


WorkbookPrintingPreview 的构造

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | 指示要打印的工作簿。 |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions 包含一些输出属性 |

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
### getEvaluatedPageCount() {#getEvaluatedPageCount--}
```
public int getEvaluatedPageCount()
```


评估此工作簿的总页数

**Example**

以下代码展示了获取工作簿页数的最快方法。

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in workbook.
         System.out.println(workbookPrintingPreview.getEvaluatedPageCount());
```

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

