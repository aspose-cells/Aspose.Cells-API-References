---
title: "WorkbookRender"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作簿渲染。"
type: docs
url: /zh/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

表示一个 Workbook 渲染。此类的构造函数必须在修改页面设置、单元格样式后使用。

**Remarks**
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | WorkbookRender 的构造 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [dispose()](#dispose--) | 释放为渲染创建和使用的资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | 获取工作簿的总页数。 |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | 获取输出图像的页面尺寸（英寸）。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | 将特定页面渲染到流中。 |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | 将特定页面渲染到流中。 |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | 将特定页面渲染到文件中。 |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | 将整个工作簿渲染为 Tiff 图像并输出到流。 |
| [toImage(String filename)](#toImage-java.lang.String-) | 将整个工作簿渲染为 Tiff 图像并输出到文件。 |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | 将工作簿渲染到打印机 |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | 将工作簿渲染到打印机 |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | 将工作簿渲染到打印机 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


WorkbookRender 的构造

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | 指示要渲染的工作簿。 |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions 包含一些输出图像的属性 |

### dispose() {#dispose--}
```
public void dispose()
```


释放为渲染创建和使用的资源。

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
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


获取工作簿的总页数。

**Returns:**
int
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


获取输出图像的页面尺寸（英寸）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | int | 页面索引从零开始。 |

**Returns:**
float[] - 图像的页面大小，[0] 为宽度，[1] 为高度
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




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


将特定页面渲染到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | int | 指示要转换的页面 |
| stream | java.io.InputStream | 输出图像的流 |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


将特定页面渲染到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | int | 指示要转换的页面 |
| stream | java.io.OutputStream | 输出图像的流 |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


将特定页面渲染到文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | int | 指示要转换的页面 |
| fileName | java.lang.String | 输出图像的文件名 |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


将整个工作簿渲染为 Tiff 图像并输出到流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 输出图像的流 |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


将整个工作簿渲染为 Tiff 图像并输出到文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filename | java.lang.String | 输出图像的文件名 |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


将工作簿渲染到打印机

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称，例如："Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


将工作簿渲染到打印机

**Remarks**

NOTE: 此方法已过时。请改用 ToPrinter(string PrinterName) 和 ImageOrPrintOptions.PageIndex、PageCount 来设置要打印的起始页和页数。此属性将在自 2021 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称，例如："Microsoft Office Document Image Writer" |
| printPageIndex | int | 要打印的第一页的基于 0 的索引，必须在范围 [0, WorkbookRender.PageCount-1] 内 |
| printPageCount | int | 要打印的页数，必须大于零 |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


将工作簿渲染到打印机

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称，例如："Microsoft Office Document Image Writer" |
| jobName | java.lang.String | 设置打印作业名称 |

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

