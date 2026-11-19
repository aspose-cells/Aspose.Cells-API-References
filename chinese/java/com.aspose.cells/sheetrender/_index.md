---
title: "SheetRender"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表渲染器，可将工作表渲染为 BMP、PNG、JPEG、TIFF 等多种图像。"
type: docs
url: /zh/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

表示工作表渲染器，可将工作表渲染为 (BMP、PNG、JPEG、TIFF…) 等多种图像。此类的构造函数必须在修改 pageSetup、单元格样式后使用。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | SheetRender 的构造，需要 worksheet 和 ImageOrPrintOptions 作为参数 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [dispose()](#dispose--) | 释放为渲染创建和使用的资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | 获取当前工作表的总页数。 |
| [getPageScale()](#getPageScale--) | 获取工作表的计算页面比例。 |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | 获取输出图像的页面尺寸（英寸）。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | 将特定页面渲染到流中。 |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | 将特定页面渲染到流中。 |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | 将特定页面渲染到文件中。 |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | 将工作表渲染到打印机 |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | 将工作表渲染到打印机 |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | 将工作表渲染到打印机 |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | 将整个工作表渲染为 Tiff 图像并输出到流。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


SheetRender 的构造，需要 worksheet 和 ImageOrPrintOptions 作为参数

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | 指示要渲染的电子表格。 |
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


获取当前工作表的总页数。

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


获取工作表的计算页面比例。如果已设置 [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--)，则返回设定的比例。否则，根据 [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) 和 [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--) 返回计算得到的比例。

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
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

**Example**

以下代码将第一张工作表的第一页输出为 png 图像。

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | int | 指示要转换的页面 |
| fileName | java.lang.String | 输出图像的文件名 |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


将工作表渲染到打印机

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称，例如："Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


将工作表渲染到打印机

**Remarks**

NOTE: 此方法已过时。请改用 ToPrinter(string PrinterName) 和 ImageOrPrintOptions.PageIndex、PageCount 来设置要打印的起始页和页数。此属性将在自 2021 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称，例如："Microsoft Office Document Image Writer" |
| printPageIndex | int | 要打印的第一页的零基索引，必须在范围 [0, SheetRender.PageCount-1] 内 |
| printPageCount | int | 要打印的页数，必须大于零 |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


将工作表渲染到打印机

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
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


将整个工作表渲染为 Tiff 图像并输出到流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 输出图像的流 |

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

