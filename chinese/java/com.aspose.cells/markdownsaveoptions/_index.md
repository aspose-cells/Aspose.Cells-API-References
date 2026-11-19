---
title: "MarkdownSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 Markdown 的保存选项。"
type: docs
url: /zh/java/com.aspose.cells/markdownsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class MarkdownSaveOptions extends SaveOptions
```

表示 Markdown 的保存选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MarkdownSaveOptions()](#MarkdownSaveOptions--) | 创建用于保存 Markdown 文档的选项 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignColumnPadding()](#getAlignColumnPadding--) | 指示是否为生成的 Markdown 表启用列对齐。 |
| [getCachedFileFolder()](#getCachedFileFolder--) | 用于临时文件的文件夹，可用作数据缓存。 |
| [getCalculateFormula()](#getCalculateFormula--) | 指示是否在保存 Markdown 文件之前计算公式。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getEncoding()](#getEncoding--) | 获取默认编码。 |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [getExportHyperlinkAsReference()](#getExportHyperlinkAsReference--) | 指示是否使用引用定义而不是内联格式导出超链接。 |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | 指定是否将图像以 Base64 格式保存到 Markdown。 |
| [getFormatStrategy()](#getFormatStrategy--) | 获取导出单元格值为字符串时的格式策略。 |
| [getImageOptions()](#getImageOptions--) | 在导出之前获取 ImageOrPrintOptions 对象。 |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | 用于在轻量模式下保存工作簿时提供单元格数据的 Data provider。 |
| [getLineSeparator()](#getLineSeparator--) | 获取换行符。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getOfficeMathOutputType()](#getOfficeMathOutputType--) | 指示 OfficeMath 对象如何导出到 Markdown，默认值为 Image。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否缓存图表的最新数据。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSheetSet()](#getSheetSet--) | 获取要渲染的工作表。 |
| [getSortExternalNames()](#getSortExternalNames--) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getSplitTablesByBlankRow()](#getSplitTablesByBlankRow--) | 指示在导出到 Markdown 时，工作表中的空行是否应视为表格分隔符。 |
| [getStreamProvider()](#getStreamProvider--) | 获取用于导出对象的 IStreamProvider。 |
| [getTableHeaderType()](#getTableHeaderType--) | 获取表格标题的设置方式。 |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | 指示是否更新 SmartArt 设置。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignColumnPadding(char value)](#setAlignColumnPadding-char-) | 指示是否为生成的 Markdown 表启用列对齐。 |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 用于临时文件的文件夹，可用作数据缓存。 |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | 指示是否在保存 Markdown 文件之前计算公式。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | 设置默认编码。 |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [setExportHyperlinkAsReference(boolean value)](#setExportHyperlinkAsReference-boolean-) | 指示是否使用引用定义而不是内联格式导出超链接。 |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | 指定是否将图像以 Base64 格式保存到 Markdown。 |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | 设置导出单元格值为字符串时的格式策略。 |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | 用于在轻量模式下保存工作簿时提供单元格数据的 Data provider。 |
| [setLineSeparator(String value)](#setLineSeparator-java.lang.String-) | 设置行分隔符。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setOfficeMathOutputType(int value)](#setOfficeMathOutputType-int-) | 指示 OfficeMath 对象如何导出到 Markdown，默认值为 Image。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否缓存图表的最新数据。 |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | 设置要渲染的工作表。 |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setSplitTablesByBlankRow(boolean value)](#setSplitTablesByBlankRow-boolean-) | 指示在导出到 Markdown 时，工作表中的空行是否应视为表格分隔符。 |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | 设置用于导出对象的 IStreamProvider。 |
| [setTableHeaderType(int value)](#setTableHeaderType-int-) | 设置表格标题的方式。 |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | 指示是否更新 SmartArt 设置。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MarkdownSaveOptions() {#MarkdownSaveOptions--}
```
public MarkdownSaveOptions()
```


创建用于保存 Markdown 文档的选项

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
### getAlignColumnPadding() {#getAlignColumnPadding--}
```
public char getAlignColumnPadding()
```


指示是否为生成的 Markdown 表格启用列对齐。启用时，列通过使用指定字符（通常为空格 ' '）填充单元格内容来对齐。将其设置为 '\\0' 可禁用列对齐（默认）。

**Returns:**
char
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


用于临时文件的文件夹，可用作数据缓存。

**Remarks**

如果未指定文件夹，则其默认值为 [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)。如果其默认值为 null 或为空，或已指定为 null 或为空，则在保存工作簿时不会使用缓存文件。

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


指示是否在保存 Markdown 文件之前计算公式。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


获取默认编码。

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

**Remarks**

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

**Returns:**
boolean
### getExportHyperlinkAsReference() {#getExportHyperlinkAsReference--}
```
public boolean getExportHyperlinkAsReference()
```


指示是否使用引用定义而非内联格式导出超链接。默认值为 false。

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


指定是否将图像以 Base64 格式保存到 Markdown。默认值为 true。

**Remarks**

当此属性设置为 true 时，图像数据直接导出到 img 元素上，不会创建单独的文件。

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


获取导出单元格值为字符串时的格式策略。

参见 [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。

**Returns:**
int
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


在导出之前获取 ImageOrPrintOptions 对象。

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


用于在轻量模式下保存工作簿时提供单元格数据的 Data provider。

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getLineSeparator() {#getLineSeparator--}
```
public String getLineSeparator()
```


获取换行符。

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getOfficeMathOutputType() {#getOfficeMathOutputType--}
```
public int getOfficeMathOutputType()
```


指示 OfficeMath 对象如何导出到 Markdown，默认值为 Image。

参见 [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype)。

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


指示是否缓存图表的最新数据。

**Returns:**
boolean
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


获取要渲染的工作表。默认是工作簿中所有可见的工作表： [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--)。

**Remarks**

当在 [SheetRender](../../com.aspose.cells/sheetrender) 中使用时，此设置将被忽略。

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
### getSplitTablesByBlankRow() {#getSplitTablesByBlankRow--}
```
public boolean getSplitTablesByBlankRow()
```


指示在导出为 Markdown 时，工作表中的空行是否应视为表格分隔符。默认值为 false。

**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


获取用于导出对象的 IStreamProvider。如果 `null`，导出的对象将保存到与输出文件相同的目录中。

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableHeaderType() {#getTableHeaderType--}
```
public int getTableHeaderType()
```


获取表格标题的设置方式。

参见 [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype)。

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlignColumnPadding(char value) {#setAlignColumnPadding-char-}
```
public void setAlignColumnPadding(char value)
```


指示是否为生成的 Markdown 表格启用列对齐。启用时，列通过使用指定字符（通常为空格 ' '）填充单元格内容来对齐。将其设置为 '\\0' 可禁用列对齐（默认）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

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

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


指示是否在保存 Markdown 文件之前计算公式。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


设置默认编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExportHyperlinkAsReference(boolean value) {#setExportHyperlinkAsReference-boolean-}
```
public void setExportHyperlinkAsReference(boolean value)
```


指示是否使用引用定义而非内联格式导出超链接。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


指定是否将图像以 Base64 格式保存到 Markdown。默认值为 true。

**Remarks**

当此属性设置为 true 时，图像数据直接导出到 img 元素上，不会创建单独的文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


设置导出单元格值为字符串时的格式策略。

参见 [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


用于在轻量模式下保存工作簿时提供单元格数据的 Data provider。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setLineSeparator(String value) {#setLineSeparator-java.lang.String-}
```
public void setLineSeparator(String value)
```


设置行分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

### setOfficeMathOutputType(int value) {#setOfficeMathOutputType-int-}
```
public void setOfficeMathOutputType(int value)
```


指示 OfficeMath 对象如何导出到 Markdown，默认值为 Image。

参见 [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype)。

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

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


设置要渲染的工作表。默认是工作簿中所有可见的工作表： [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--)。

**Remarks**

当在 [SheetRender](../../com.aspose.cells/sheetrender) 中使用时，此设置将被忽略。

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

### setSplitTablesByBlankRow(boolean value) {#setSplitTablesByBlankRow-boolean-}
```
public void setSplitTablesByBlankRow(boolean value)
```


指示在导出为 Markdown 时，工作表中的空行是否应视为表格分隔符。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


设置用于导出对象的 IStreamProvider。如果 `null`，导出的对象将保存到与输出文件相同的目录中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableHeaderType(int value) {#setTableHeaderType-int-}
```
public void setTableHeaderType(int value)
```


设置表格标题的方式。

参见 [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype)。

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

