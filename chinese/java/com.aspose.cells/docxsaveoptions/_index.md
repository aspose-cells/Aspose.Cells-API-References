---
title: "DocxSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示保存 .docx 文件的选项。"
type: docs
url: /zh/java/com.aspose.cells/docxsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class DocxSaveOptions extends PaginatedSaveOptions
```

表示保存 .docx 文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocxSaveOptions()](#DocxSaveOptions--) | 表示保存 .docx 文件的选项。 |
| [DocxSaveOptions(boolean saveAsImage)](#DocxSaveOptions-boolean-) | 表示保存 .docx 文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果中的一页。 |
| [getAsFlatOpc()](#getAsFlatOpc--) | 指示是否将保存为可以由 Open XML SDK 生成的平面 OPC 文件。 |
| [getAsNormalView()](#getAsNormalView--) | 将 Excel 文件导出为普通视图的 docx 文件。 |
| [getCachedFileFolder()](#getCachedFileFolder--) | 用于临时文件的文件夹，可用作数据缓存。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | 指示是否检查文本中每个字符的字体兼容性。 |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | 获取渲染期间的自定义设置。 |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | 获取默认编辑语言。 |
| [getDefaultFont()](#getDefaultFont--) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [getEmbedXlsxAsChartDataSource()](#getEmbedXlsxAsChartDataSource--) | 指示是否将 xlsx 文件嵌入为图表的数据源。 |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | 用于渲染 Emf 元文件的设置。 |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [getGridlineColor()](#getGridlineColor--) | 获取网格线颜色。 |
| [getGridlineType()](#getGridlineType--) | 获取网格线类型。 |
| [getIgnoreError()](#getIgnoreError--) | 指示是否需要在渲染时隐藏错误。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将仅输出到结果中的一页。 |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | 指示在没有可打印内容时是否输出空白页。 |
| [getPageCount()](#getPageCount--) | 获取要保存的页数。 |
| [getPageIndex()](#getPageIndex--) | 获取要保存的第一页的基于 0 的索引。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 控制/指示页面保存过程的进度。 |
| [getPrintingPageType()](#getPrintingPageType--) | 指示哪些页面将不会被打印。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否缓存图表的最新数据。 |
| [getRenderingBehavior()](#getRenderingBehavior--) | 获取要应用的 Excel 特定渲染行为。 |
| [getSaveAsEditableShapes()](#getSaveAsEditableShapes--) | 将所有绘图对象保存为 Word 文件中的可编辑形状，以便您可以在 Word 中编辑它们。 |
| [getSaveAsEditableShaps()](#getSaveAsEditableShaps--) | 将所有绘图对象保存为 Word 文件中的可编辑形状。这样您可以在 Word 中编辑它们。 |
| [getSaveElementType()](#getSaveElementType--) | 指示应保存哪些元素。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSheetSet()](#getSheetSet--) | 获取要渲染的工作表。 |
| [getSortExternalNames()](#getSortExternalNames--) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getTextCrossType()](#getTextCrossType--) | 获取当文本宽度大于单元格宽度时的显示文本类型。 |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | 指示是否更新 SmartArt 设置。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | 指示当单元格字体与字符不兼容时是否仅替换该字符的字体。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果中的一页。 |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | 指示是否将保存为可以由 Open XML SDK 生成的平面 OPC 文件。 |
| [setAsNormalView(boolean value)](#setAsNormalView-boolean-) | 将 Excel 文件导出为普通视图的 docx 文件。 |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 用于临时文件的文件夹，可用作数据缓存。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | 指示是否检查文本中每个字符的字体兼容性。 |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | 设置渲染期间的自定义设置。 |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | 设置默认编辑语言。 |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [setEmbedXlsxAsChartDataSource(boolean value)](#setEmbedXlsxAsChartDataSource-boolean-) | 指示是否将 xlsx 文件嵌入为图表的数据源。 |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | 用于渲染 Emf 元文件的设置。 |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | 指示当单元格字体与字符不兼容时是否仅替换该字符的字体。 |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | 设置网格线颜色。 |
| [setGridlineType(int value)](#setGridlineType-int-) | 设置网格线类型。 |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | 指示是否需要在渲染时隐藏错误。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将仅输出到结果中的一页。 |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | 指示在没有可打印内容时是否输出空白页。 |
| [setPageCount(int value)](#setPageCount-int-) | 设置要保存的页数。 |
| [setPageIndex(int value)](#setPageIndex-int-) | 设置要保存的第一页的基于 0 的索引。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | 控制/指示页面保存过程的进度。 |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | 指示哪些页面将不会被打印。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否缓存图表的最新数据。 |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | 设置要应用的 Excel 特定渲染行为。 |
| [setSaveAsEditableShapes(boolean value)](#setSaveAsEditableShapes-boolean-) | 将所有绘图对象保存为 Word 文件中的可编辑形状，以便您可以在 Word 中编辑它们。 |
| [setSaveAsEditableShaps(boolean value)](#setSaveAsEditableShaps-boolean-) | 将所有绘图对象保存为 Word 文件中的可编辑形状。这样您可以在 Word 中编辑它们。 |
| [setSaveElementType(int value)](#setSaveElementType-int-) | 指示应保存哪些元素。 |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | 设置要渲染的工作表。 |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setTextCrossType(int value)](#setTextCrossType-int-) | 当文本宽度大于单元格宽度时，设置显示文本的类型。 |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | 指示是否更新 SmartArt 设置。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DocxSaveOptions() {#DocxSaveOptions--}
```
public DocxSaveOptions()
```


表示保存 .docx 文件的选项。

### DocxSaveOptions(boolean saveAsImage) {#DocxSaveOptions-boolean-}
```
public DocxSaveOptions(boolean saveAsImage)
```


表示保存 .docx 文件的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveAsImage | boolean | 如果为 True，工作簿将转换为 .docx 文件中的图片。若为 False，工作簿将转换为 .docx 文件中的表格。 |

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


如果 AllColumnsInOnePagePerSheet 为 true，则单个工作表的所有列内容将仅输出到结果的一个页面。页面设置的纸张宽度将被忽略，页面设置的其他设置仍然生效。

**Returns:**
boolean
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


指示是否将保存为可以由 Open XML SDK 生成的平面 OPC 文件。

**Returns:**
boolean
### getAsNormalView() {#getAsNormalView--}
```
public boolean getAsNormalView()
```


将 Excel 文件导出为普通视图的 docx 文件。如果此属性为 true，将输出一个区域，且不适用缩放。默认值为 false。

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


用于临时文件的文件夹，可用作数据缓存。

**Remarks**

如果未指定文件夹，则其默认值为 [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)。如果其默认值为 null 或为空，或已指定为 null 或为空，则在保存工作簿时不会使用缓存文件。

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


指示是否检查文本中每个字符的字体兼容性。

**Remarks**

默认值为 true。禁用此属性可能会提升性能。但当默认或指定的文本/字符字体无法用于渲染时，生成的 PDF 可能出现不可读的字符（如方块）。在这种情况下，用户应保持此属性为 true，以便搜索并使用替代字体来渲染文本。

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试使用工作簿的默认字体首先显示这些字符。

**Remarks**

默认值为 true。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


在保存文件后使工作簿为空。

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


如果为 true 且目录不存在，目录将在保存文件之前自动创建。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


获取渲染期间的自定义设置。

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


获取默认编辑语言。

参见 [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage)。

**Remarks**

当设置不同的编辑语言时，可能会显示/渲染文本段落的不同布局。默认值为 [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO)。

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


实现此接口以在渲染时获取 DrawObject 和 Bound。

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedXlsxAsChartDataSource() {#getEmbedXlsxAsChartDataSource--}
```
public boolean getEmbedXlsxAsChartDataSource()
```


指示是否将 xlsx 文件嵌入为图表的数据源。

**Remarks**

默认值为 true。

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


用于渲染 Emf 元文件的设置。

参见 [EmfRenderSetting](../../com.aspose.cells/emfrendersetting)。

**Remarks**

EMF 元文件标识为 \"EMF+ Dual\" 可以同时包含 EMF+ 记录和 EMF 记录。可以使用任意类型的记录来渲染图像，或仅使用 EMF+ 记录，或仅使用 EMF 记录。当设置 [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) 时，渲染到页面时将解析 EMF+ 记录，否则仅解析 EMF 记录。默认值为 [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)。

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

**Remarks**

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


获取网格线颜色。

**Remarks**

它将忽略源文件中的网格线颜色设置。

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


获取网格线类型。

参见 [GridlineType](../../com.aspose.cells/gridlinetype)。

**Remarks**

默认值为 Dotted 类型。

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面。

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


如果 OnePagePerSheet 为 true，则单个工作表的所有内容将仅输出到结果的一个页面。页面设置的纸张大小将失效，页面设置的其他设置仍然生效。

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


指示在没有可打印内容时是否输出空白页。

**Remarks**

默认值为 true。

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


获取要保存的页数。

**Remarks**

默认值为 System.Int32.MaxValue，表示将渲染所有页面。

**Example**

以下示例展示了如何将 Microsoft Excel 文件中的页面范围（第 3 页和第 4 页）渲染为 PDF。

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


获取要保存的第一页的基于 0 的索引。

**Remarks**

默认值为 0。

**Example**

以下示例展示了如何将 Microsoft Excel 文件中的页面范围（第 3 页和第 4 页）渲染为 PDF。

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


控制/指示页面保存过程的进度。

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


指示哪些页面将不会被打印。

参见 [PrintingPageType](../../com.aspose.cells/printingpagetype)。

**Remarks**

如果工作表中的内容稀疏，输出的 PDF 文件中可能会出现完全空白的页面。如果您不想要这些空白页，可以使用此选项将其省略。

**Example**

以下代码会省略空白页或仅包含单元格背景、边框等样式内容的页面。

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


指示是否缓存图表的最新数据。

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


获取要应用的 Excel 特定渲染行为。

参见 [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior)。

**Remarks**

默认值为 [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL)。

**Returns:**
int
### getSaveAsEditableShapes() {#getSaveAsEditableShapes--}
```
public boolean getSaveAsEditableShapes()
```


将所有绘图对象保存为 Word 文件中的可编辑形状，以便您可以在 Word 中编辑它们。

**Remarks**

仅适用于图表。

**Returns:**
boolean
### getSaveAsEditableShaps() {#getSaveAsEditableShaps--}
```
public boolean getSaveAsEditableShaps()
```


将所有绘图对象保存为 Word 文件中的可编辑形状。这样您可以在 Word 中编辑它们。

**Remarks**

注意：此成员已过时。请改用 [getSaveAsEditableShapes()](../../com.aspose.cells/docxsaveoptions\#getSaveAsEditableShapes--) 属性。该属性将在自 2025 年 5 月起的 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getSaveElementType() {#getSaveElementType--}
```
public int getSaveElementType()
```


指示应保存哪些元素。

参见 [SaveElementType](../../com.aspose.cells/saveelementtype)。

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取保存的文件格式。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


获取要渲染的工作表。默认是工作簿中所有可见工作表：[SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--)。

**Example**

以下代码仅将活动工作表渲染为 pdf。

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


指示在保存文件之前是否对外部已定义名称进行排序。

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


指示在保存文件之前是否对已定义名称进行排序。

**Returns:**
boolean
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


获取当文本宽度大于单元格宽度时的显示文本类型。

请参阅 [TextCrossType](../../com.aspose.cells/textcrosstype)。

**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


指示是否更新 Smart Art 设置。默认值为 false。

**Remarks**

仅在调用 Shape.GetResultOfSmartArt() 方法且模板文件中存在缓存形状后生效。

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


指示在保存文件之前是否验证合并的单元格。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


获取警告回调。

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


指示当单元格字体与字符不兼容时是否仅替换该字符的字体。

**Remarks**

默认值为 false。我们将首先尝试 Workbook 的默认字体以及 PdfSaveOption/system 用于单元格字体。

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


如果 AllColumnsInOnePagePerSheet 为 true，则单个工作表的所有列内容将仅输出到结果的一个页面。页面设置的纸张宽度将被忽略，页面设置的其他设置仍然生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


指示是否将保存为可以由 Open XML SDK 生成的平面 OPC 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAsNormalView(boolean value) {#setAsNormalView-boolean-}
```
public void setAsNormalView(boolean value)
```


将 Excel 文件导出为普通视图的 docx 文件。如果此属性为 true，将输出一个区域，且不适用缩放。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


用于临时文件的文件夹，可用作数据缓存。

**Remarks**

如果未指定文件夹，则其默认值为 [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)。如果其默认值为 null 或为空，或已指定为 null 或为空，则在保存工作簿时不会使用缓存文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


指示是否检查文本中每个字符的字体兼容性。

**Remarks**

默认值为 true。禁用此属性可能会提升性能。但当默认或指定的文本/字符字体无法用于渲染时，生成的 PDF 可能出现不可读的字符（如方块）。在这种情况下，用户应保持此属性为 true，以便搜索并使用替代字体来渲染文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试使用工作簿的默认字体首先显示这些字符。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


在保存文件后使工作簿为空。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


如果为 true 且目录不存在，目录将在保存文件之前自动创建。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


设置渲染期间的自定义设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


设置默认编辑语言。

参见 [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage)。

**Remarks**

当设置不同的编辑语言时，可能会显示/渲染文本段落的不同布局。默认值为 [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


实现此接口以在渲染时获取 DrawObject 和 Bound。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedXlsxAsChartDataSource(boolean value) {#setEmbedXlsxAsChartDataSource-boolean-}
```
public void setEmbedXlsxAsChartDataSource(boolean value)
```


指示是否将 xlsx 文件嵌入为图表的数据源。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


用于渲染 Emf 元文件的设置。

参见 [EmfRenderSetting](../../com.aspose.cells/emfrendersetting)。

**Remarks**

EMF 元文件标识为 \"EMF+ Dual\" 可以同时包含 EMF+ 记录和 EMF 记录。可以使用任意类型的记录来渲染图像，或仅使用 EMF+ 记录，或仅使用 EMF 记录。当设置 [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) 时，渲染到页面时将解析 EMF+ 记录，否则仅解析 EMF 记录。默认值为 [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

**Remarks**

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


指示当单元格字体与字符不兼容时是否仅替换该字符的字体。

**Remarks**

默认值为 false。我们将首先尝试 Workbook 的默认字体以及 PdfSaveOption/system 用于单元格字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


设置网格线颜色。

**Remarks**

它将忽略源文件中的网格线颜色设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


设置网格线类型。

参见 [GridlineType](../../com.aspose.cells/gridlinetype)。

**Remarks**

默认值为 Dotted 类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


如果 OnePagePerSheet 为 true，则单个工作表的所有内容将仅输出到结果的一个页面。页面设置的纸张大小将失效，页面设置的其他设置仍然生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


指示在没有可打印内容时是否输出空白页。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


设置要保存的页数。

**Remarks**

默认值为 System.Int32.MaxValue，表示将渲染所有页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


设置要保存的第一页的基于 0 的索引。

**Remarks**

默认值为 0。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


控制/指示页面保存过程的进度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


指示哪些页面将不会被打印。

参见 [PrintingPageType](../../com.aspose.cells/printingpagetype)。

**Remarks**

如果工作表中的内容稀疏，输出的 PDF 文件中可能会出现完全空白的页面。如果您不想要这些空白页，可以使用此选项将其省略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


指示是否缓存图表的最新数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


设置要应用的 Excel 特定渲染行为。

参见 [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior)。

**Remarks**

默认值为 [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSaveAsEditableShapes(boolean value) {#setSaveAsEditableShapes-boolean-}
```
public void setSaveAsEditableShapes(boolean value)
```


将所有绘图对象保存为 Word 文件中的可编辑形状，以便您可以在 Word 中编辑它们。

**Remarks**

仅适用于图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveAsEditableShaps(boolean value) {#setSaveAsEditableShaps-boolean-}
```
public void setSaveAsEditableShaps(boolean value)
```


将所有绘图对象保存为 Word 文件中的可编辑形状。这样您可以在 Word 中编辑它们。

**Remarks**

注意：此成员已过时。请改用 [getSaveAsEditableShapes()](../../com.aspose.cells/docxsaveoptions\#getSaveAsEditableShapes--) 属性。该属性将在自 2025 年 5 月起的 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveElementType(int value) {#setSaveElementType-int-}
```
public void setSaveElementType(int value)
```


指示应保存哪些元素。

参见 [SaveElementType](../../com.aspose.cells/saveelementtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


设置要渲染的工作表。默认是工作簿中所有可见工作表：[SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


指示在保存文件之前是否对外部已定义名称进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


指示在保存文件之前是否对已定义名称进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


当文本宽度大于单元格宽度时，设置显示文本的类型。

请参阅 [TextCrossType](../../com.aspose.cells/textcrosstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


指示是否更新 Smart Art 设置。默认值为 false。

**Remarks**

仅在调用 Shape.GetResultOfSmartArt() 方法且模板文件中存在缓存形状后生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


指示在保存文件之前是否验证合并的单元格。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


设置警告回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

