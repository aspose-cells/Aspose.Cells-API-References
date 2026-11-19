---
title: "PageSetup"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示页面设置描述的对象。"
type: docs
url: /zh/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

封装表示页面设置描述的对象。PageSetup 对象包含所有页面设置选项。

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | 清除页眉和页脚设置。 |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | 复制页面设置的设置。 |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | 设置自定义纸张尺寸，单位为英寸。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | 表示文档元素是否以黑白方式打印。 |
| [getBottomMargin()](#getBottomMargin--) | 表示底部边距的大小，单位为厘米。 |
| [getBottomMarginInch()](#getBottomMarginInch--) | 表示底部边距的大小，单位为英寸。 |
| [getCenterHorizontally()](#getCenterHorizontally--) | 表示工作表是否水平居中打印。 |
| [getCenterVertically()](#getCenterVertically--) | 表示工作表是否垂直居中打印。 |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | 获取页眉或页脚的所有命令。 |
| [getEvenFooter(int section)](#getEvenFooter-int-) | 获取用于格式化 Excel 文件偶数页页脚的脚本。 |
| [getEvenHeader(int section)](#getEvenHeader-int-) | 获取用于格式化 Excel 文件偶数页页眉的脚本。 |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | 获取用于格式化 Excel 文件首页页脚的脚本。 |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | 获取用于格式化 Excel 文件首页页眉的脚本。 |
| [getFirstPageNumber()](#getFirstPageNumber--) | 表示打印此工作表时使用的起始页码。 |
| [getFitToPagesTall()](#getFitToPagesTall--) | 表示打印时工作表在纵向上缩放至的页数。 |
| [getFitToPagesWide()](#getFitToPagesWide--) | 表示打印时工作表在横向上缩放至的页数。 |
| [getFooter(int section)](#getFooter-int-) | 获取用于格式化 Excel 文件页脚的脚本。 |
| [getFooterMargin()](#getFooterMargin--) | 表示页面底部到页脚的距离，单位为厘米。 |
| [getFooterMarginInch()](#getFooterMarginInch--) | 表示页面底部到页脚的距离，单位为英寸。 |
| [getHeader(int section)](#getHeader-int-) | 获取用于格式化 Excel 文件标题的脚本。 |
| [getHeaderMargin()](#getHeaderMargin--) | 表示页面顶部到页眉的距离，单位为厘米。 |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | 表示页面顶部到页眉的距离，单位为英寸。 |
| [getLeftMargin()](#getLeftMargin--) | 表示左边距的大小，单位为厘米。 |
| [getLeftMarginInch()](#getLeftMarginInch--) | 表示左边距的大小，单位为英寸。 |
| [getODSPageBackground()](#getODSPageBackground--) | 获取 ODS 的背景。 |
| [getOrder()](#getOrder--) | 表示 Microsoft Excel 在打印大型工作表时用于给页码排序的顺序。 |
| [getOrientation()](#getOrientation--) | 表示页面打印方向。 |
| [getPaperHeight()](#getPaperHeight--) | 获取纸张的高度，单位为英寸，考虑页面方向。 |
| [getPaperSize()](#getPaperSize--) | 表示纸张的大小。 |
| [getPaperWidth()](#getPaperWidth--) | 获取纸张的宽度，单位为英寸，考虑页面方向。 |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | 获取页眉/页脚的 [Picture](../../com.aspose.cells/picture) 对象。 |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | 获取页眉/页脚的 [Picture](../../com.aspose.cells/picture) 对象。 |
| [getPrintArea()](#getPrintArea--) | 表示要打印的范围。 |
| [getPrintComments()](#getPrintComments--) | 表示注释随工作表的打印方式。 |
| [getPrintCopies()](#getPrintCopies--) | 获取要打印的副本数量。 |
| [getPrintDraft()](#getPrintDraft--) | 表示工作表是否将在没有图形的情况下打印。 |
| [getPrintErrors()](#getPrintErrors--) | 指定显示的打印错误类型。 |
| [getPrintGridlines()](#getPrintGridlines--) | 表示是否在页面上打印单元格网格线。 |
| [getPrintHeadings()](#getPrintHeadings--) | 表示是否在此页面上打印行和列标题。 |
| [getPrintQuality()](#getPrintQuality--) | 表示打印质量。 |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | 表示包含要在每页左侧重复的单元格的列。 |
| [getPrintTitleRows()](#getPrintTitleRows--) | 表示包含要在每页顶部重复的单元格的行。 |
| [getPrinterSettings()](#getPrinterSettings--) | 获取默认打印机的设置。 |
| [getRightMargin()](#getRightMargin--) | 表示右边距的大小，单位为厘米。 |
| [getRightMarginInch()](#getRightMarginInch--) | 表示右边距的大小，单位为英寸。 |
| [getTopMargin()](#getTopMargin--) | 表示顶部边距的大小，单位为厘米。 |
| [getTopMarginInch()](#getTopMarginInch--) | 表示顶部边距的大小，单位为英寸。 |
| [getZoom()](#getZoom--) | 表示以百分比计的缩放因子。 |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | 指示是否自动分配首页的页码。 |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | 指示纸张尺寸是否自动。 |
| [isHFAlignMargins()](#isHFAlignMargins--) | 指示页眉和页脚的边距是否与页面边距对齐。 |
| [isHFDiffFirst()](#isHFDiffFirst--) | True 表示首页的页眉/页脚与其他页面不同。 |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | True 表示奇数页的页眉/页脚与奇数页不同。 |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | 指示页眉和页脚是否随文档缩放而缩放。 |
| [isPercentScale()](#isPercentScale--) | 如果此属性为 False，则 FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | 指示是否自动分配首页的页码。 |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | 表示文档元素是否以黑白方式打印。 |
| [setBottomMargin(double value)](#setBottomMargin-double-) | 表示底部边距的大小，单位为厘米。 |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | 表示底部边距的大小，单位为英寸。 |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | 表示工作表是否水平居中打印。 |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | 表示工作表是否垂直居中打印。 |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | 设置用于 Excel 文件偶数页页脚的脚本格式。 |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | 设置用于 Excel 文件偶数页页眉的脚本格式。 |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | 设置用于 Excel 文件首页页脚的脚本格式。 |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | 设置用于 Excel 文件首页页眉的脚本格式。 |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | 表示打印此工作表时使用的起始页码。 |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | 设置工作表在打印时将被缩放到的页数。 |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | 表示打印时工作表在纵向上缩放至的页数。 |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | 表示打印时工作表在横向上缩放至的页数。 |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | 设置用于 Excel 文件页脚的脚本格式。 |
| [setFooterMargin(double value)](#setFooterMargin-double-) | 表示页面底部到页脚的距离，单位为厘米。 |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | 表示页面底部到页脚的距离，单位为英寸。 |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | 在工作表的页脚中设置图像。 |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | 指示页眉和页脚的边距是否与页面边距对齐。 |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | True 表示首页的页眉/页脚与其他页面不同。 |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | True 表示奇数页的页眉/页脚与奇数页不同。 |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | 指示页眉和页脚是否随文档缩放而缩放。 |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | 设置用于 Excel 文件页眉的脚本格式。 |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | 表示页面顶部到页眉的距离，单位为厘米。 |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | 表示页面顶部到页眉的距离，单位为英寸。 |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | 在工作表的页眉中设置图像。 |
| [setLeftMargin(double value)](#setLeftMargin-double-) | 表示左边距的大小，单位为厘米。 |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | 表示左边距的大小，单位为英寸。 |
| [setOrder(int value)](#setOrder-int-) | 表示 Microsoft Excel 在打印大型工作表时用于给页码排序的顺序。 |
| [setOrientation(int value)](#setOrientation-int-) | 表示页面打印方向。 |
| [setPaperSize(int value)](#setPaperSize-int-) | 表示纸张的大小。 |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | 如果此属性为 False，则 FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。 |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | 在工作表的页眉/页脚中设置图像。 |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | 表示要打印的范围。 |
| [setPrintComments(int value)](#setPrintComments-int-) | 表示注释随工作表的打印方式。 |
| [setPrintCopies(int value)](#setPrintCopies-int-) | 设置打印的副本数量。 |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | 表示工作表是否将在没有图形的情况下打印。 |
| [setPrintErrors(int value)](#setPrintErrors-int-) | 指定显示的打印错误类型。 |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | 表示是否在页面上打印单元格网格线。 |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | 表示是否在此页面上打印行和列标题。 |
| [setPrintQuality(int value)](#setPrintQuality-int-) | 表示打印质量。 |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | 表示包含要在每页左侧重复的单元格的列。 |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | 表示包含要在每页顶部重复的单元格的行。 |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | 设置默认打印机的设置。 |
| [setRightMargin(double value)](#setRightMargin-double-) | 表示右边距的大小，单位为厘米。 |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | 表示右边距的大小，单位为英寸。 |
| [setTopMargin(double value)](#setTopMargin-double-) | 表示顶部边距的大小，单位为厘米。 |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | 表示顶部边距的大小，单位为英寸。 |
| [setZoom(int value)](#setZoom-int-) | 表示以百分比计的缩放因子。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


清除页眉和页脚设置。

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


复制页面设置的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | 来源。 |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | 复制选项。 |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


设置自定义纸张尺寸，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 宽度 | double | 纸张的宽度。 |
| 高度 | double | 纸张的高度。 |

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
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


表示文档元素是否以黑白方式打印。

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


表示底部边距的大小，单位为厘米。

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


表示底部边距的大小，单位为英寸。

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


表示工作表是否水平居中打印。

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


表示工作表是否垂直居中打印。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


获取页眉或页脚的所有命令。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| headerFooterScript | java.lang.String | 页眉/页脚脚本 |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - 返回页眉或页脚的所有命令。
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


获取用于格式化 Excel 文件偶数页页脚的脚本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


获取用于格式化 Excel 文件偶数页页眉的脚本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


获取用于格式化 Excel 文件首页页脚的脚本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


获取用于格式化 Excel 文件首页页眉的脚本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


表示打印此工作表时使用的起始页码。

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


表示打印时工作表将缩放到的页数高度。默认值为 1。

**Remarks**

如果希望所有行适合在一页上，必须将 FitToPagesWide 设置为零。

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


表示打印时工作表将缩放到的页数宽度。默认值为 1。

**Remarks**

如果希望所有列适合在一页上，必须将 FitToPagesTall 设置为零。

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


获取用于格式化 Excel 文件页脚的脚本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


表示页面底部到页脚的距离，单位为厘米。

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


表示页面底部到页脚的距离，单位为英寸。

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


获取用于格式化 Excel 文件标题的脚本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


表示页面顶部到页眉的距离，单位为厘米。

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


表示页面顶部到页眉的距离，单位为英寸。

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


表示左边距的大小，单位为厘米。

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


表示左边距的大小，单位为英寸。

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


获取 ODS 的背景。

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


表示 Microsoft Excel 在打印大型工作表时用于给页码排序的顺序。

参见 [PrintOrderType](../../com.aspose.cells/printordertype)。

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


表示页面打印方向。

请参阅 [PageOrientationType](../../com.aspose.cells/pageorientationtype)。

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


获取纸张的高度，单位为英寸，考虑页面方向。

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


表示纸张的大小。

参见 [PaperSizeType](../../com.aspose.cells/papersizetype)。

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


获取纸张的宽度，单位为英寸，考虑页面方向。

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


获取页眉/页脚的 [Picture](../../com.aspose.cells/picture) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isFirst | boolean | 指示是否获取首页页眉/页脚的图片。 |
| isEven | boolean | 指示是否获取偶数页页眉/页脚的图片。 |
| isHeader | boolean | 指示是否获取页眉/页脚的图片。 |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


获取页眉/页脚的 [Picture](../../com.aspose.cells/picture) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isHeader | boolean | 指示它是在页眉还是页脚中。 |
| 节 | int | 0：左节，1：中节，2：右节。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


表示要打印的范围。

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


表示注释随工作表的打印方式。

参见 [PrintCommentsType](../../com.aspose.cells/printcommentstype)。

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


获取要打印的副本数量。

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


表示工作表是否将在没有图形的情况下打印。

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


指定显示的打印错误类型。

请参阅 [PrintErrorsType](../../com.aspose.cells/printerrorstype)。

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


表示是否在页面上打印单元格网格线。

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


表示是否在此页面上打印行和列标题。

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


表示打印质量。

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


表示包含要在每页左侧重复的单元格的列。

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


表示包含要在每页顶部重复的单元格的行。

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


获取默认打印机的设置。

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


表示右边距的大小，单位为厘米。

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


表示右边距的大小，单位为英寸。

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


表示顶部边距的大小，单位为厘米。

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


表示顶部边距的大小，单位为英寸。

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


表示以百分比计的缩放因子。取值应在 10 到 400 之间。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


指示是否自动分配首页的页码。

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


指示纸张尺寸是否自动。

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


指示页眉和页脚的边距是否与页面边距对齐。如果此属性为 true，左侧页眉和页脚将与左边距对齐，右侧页眉和页脚将与右边距对齐。此选项默认启用。

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


True 表示首页的页眉/页脚与其他页面不同。

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


True 表示奇数页的页眉/页脚与奇数页不同。

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


指示页眉和页脚是否随文档缩放而缩放。仅适用于 Excel 2007。

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


如果此属性为 False，则 FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


指示是否自动分配首页的页码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


表示文档元素是否以黑白方式打印。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


表示底部边距的大小，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


表示底部边距的大小，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


表示工作表是否水平居中打印。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


表示工作表是否垂直居中打印。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


设置用于格式化 Excel 文件偶数页页脚的脚本。仅在 Excel 2007 且 IsHFDiffOddEven 为 true 时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| footerScript | java.lang.String | 页脚格式脚本。 |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


设置用于格式化 Excel 文件偶数页页眉的脚本。仅在 Excel 2007 且 IsHFDiffOddEven 为 true 时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| headerScript | java.lang.String | 标题格式脚本。 |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


设置用于 Excel 文件首页页脚的脚本格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| footerScript | java.lang.String | 页脚格式脚本。 |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


设置一个脚本，用于格式化 Excel 文件的首页页眉。仅在 Excel 2007 且 IsHFDiffFirst 为 true 时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| headerScript | java.lang.String | 标题格式脚本。 |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


表示打印此工作表时使用的起始页码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


设置工作表在打印时将被缩放到的页数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 宽 | int | 页宽。 |
| 高 | int | 页高。 |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


表示打印时工作表将缩放到的页数高度。默认值为 1。

**Remarks**

如果希望所有行适合在一页上，必须将 FitToPagesWide 设置为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


表示打印时工作表将缩放到的页数宽度。默认值为 1。

**Remarks**

如果希望所有列适合在一页上，必须将 FitToPagesTall 设置为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


设置用于 Excel 文件页脚的脚本格式。

**Remarks**

脚本命令：

| 命令 | 描述 |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | 当前页码\u9286\u20ac |
| &N | 页数\u9286\u20ac |
| &D | 当前日期\u9286\u20ac |
| &T | 当前时间 |
| &A | 工作表名称 |
| &F | 不含路径的文件名 |
| &"<FontName>" | 字体名称，例如：&"Arial" |
| &"<FontName>, <FontStyle>" | 字体名称和字体样式，例如：&"Arial,Bold" |
| &<FontSize> | 字体大小。如果此命令后跟一个普通数字用于在页眉中打印，它将与字体高度之间用空格字符分隔。 |
| &K<RRGGBB> | 字体颜色，例如（红色）：&KFF0000 |
| &G | 图像脚本 |

例如："&Arial,Bold&8Footer Note"

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| footerScript | java.lang.String | 页脚格式脚本。 |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


表示页面底部到页脚的距离，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


表示页面底部到页脚的距离，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


在工作表的页脚中设置图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| footerPicture | byte[] | 图像数据。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


指示页眉和页脚的边距是否与页面边距对齐。如果此属性为 true，左侧页眉和页脚将与左边距对齐，右侧页眉和页脚将与右边距对齐。此选项默认启用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


True 表示首页的页眉/页脚与其他页面不同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


True 表示奇数页的页眉/页脚与奇数页不同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


指示页眉和页脚是否随文档缩放而缩放。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


设置用于 Excel 文件页眉的脚本格式。

**Remarks**

脚本命令：

| 命令 | 描述 |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | 当前页码\u9286\u20ac |
| &N | 页数\u9286\u20ac |
| &D | 当前日期\u9286\u20ac |
| &T | 当前时间 |
| &A | 工作表名称 |
| &F | 不含路径的文件名 |
| &"<FontName>" | 字体名称，例如：&"Arial" |
| &"<FontName>, <FontStyle>" | 字体名称和字体样式，例如：&"Arial,Bold" |
| &<FontSize> | 字体大小。如果此命令后跟一个普通数字用于在页眉中打印，它将与字体高度之间用空格字符分隔。 |
| &K<RRGGBB> | 字体颜色，例如（红色）：&KFF0000 |
| &G | 图像脚本 |

例如："&Arial,Bold&8Header Note"

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| headerScript | java.lang.String | 标题格式脚本。 |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


表示页面顶部到页眉的距离，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


表示页面顶部到页眉的距离，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


在工作表的页眉中设置图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节 | int | 0：左节，1：中节，2：右节。 |
| headerPicture | byte[] | 图像数据。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


表示左边距的大小，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


表示左边距的大小，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


表示 Microsoft Excel 在打印大型工作表时用于给页码排序的顺序。

参见 [PrintOrderType](../../com.aspose.cells/printordertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


表示页面打印方向。

请参阅 [PageOrientationType](../../com.aspose.cells/pageorientationtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


表示纸张的大小。

参见 [PaperSizeType](../../com.aspose.cells/papersizetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


如果此属性为 False，则 FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


在工作表的页眉/页脚中设置图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isFirst | boolean | 指示是否设置首页页眉/页脚的图片。 |
| isEven | boolean | 指示是否设置偶数页页眉/页脚的图片。 |
| isHeader | boolean | 指示是否设置页眉/页脚的图片。 |
| 节 | int | 0：左节，1：中节，2：右节。 |
| imageData | byte[] | 图像数据。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


表示要打印的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


表示注释随工作表的打印方式。

参见 [PrintCommentsType](../../com.aspose.cells/printcommentstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


设置打印的副本数量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


表示工作表是否将在没有图形的情况下打印。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


指定显示的打印错误类型。

请参阅 [PrintErrorsType](../../com.aspose.cells/printerrorstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


表示是否在页面上打印单元格网格线。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


表示是否在此页面上打印行和列标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


表示打印质量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


表示包含要在每页左侧重复的单元格的列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


表示包含要在每页顶部重复的单元格的行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


设置默认打印机的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


表示右边距的大小，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


表示右边距的大小，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


表示顶部边距的大小，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


表示顶部边距的大小，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


表示以百分比计的缩放因子。取值应在 10 到 400 之间。

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

