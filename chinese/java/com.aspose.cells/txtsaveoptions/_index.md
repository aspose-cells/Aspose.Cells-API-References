---
title: "TxtSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 csv/制表符分隔/其他文本格式的保存选项。"
type: docs
url: /zh/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

表示 csv/制表符分隔/其他文本格式的保存选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | 创建文本文件保存选项。 |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | 创建文本文件保存选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | 指示是否始终为每个字段添加 '"'。 |
| [getCachedFileFolder()](#getCachedFileFolder--) | 用于临时文件的文件夹，可用作数据缓存。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getEncoding()](#getEncoding--) | 获取默认编码。 |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [getExportAllSheets()](#getExportAllSheets--) | 指示是否将所有工作表导出到文本文件。 |
| [getExportArea()](#getExportArea--) | 要导出的单元格范围。 |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | 指示当 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 为 true 时，是否应将单引号符号作为单元格值的一部分导出。 |
| [getFormatStrategy()](#getFormatStrategy--) | 获取导出单元格值为字符串时的格式策略。 |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | 指示是否应为空行输出分隔符。 |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | 用于在轻量模式下保存工作簿的数据提供程序。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getQuoteType()](#getQuoteType--) | 获取在导出文本文件中如何引用值。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否缓存图表的最新数据。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSeparator()](#getSeparator--) | 获取文本文件的字符分隔符。 |
| [getSeparatorString()](#getSeparatorString--) | 获取字符串值作为分隔符。 |
| [getSortExternalNames()](#getSortExternalNames--) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | 指示是否应像 Microsoft Excel 那样修剪前导空行和空列。 |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | 指示是否应修剪一行中尾随的空单元格。 |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | 指示是否更新 SmartArt 设置。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | 指示是否始终为每个字段添加 '"'。 |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 用于临时文件的文件夹，可用作数据缓存。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | 设置默认编码。 |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | 指示是否将所有工作表导出到文本文件。 |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | 要导出的单元格范围。 |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | 指示当 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 为 true 时，是否应将单引号符号作为单元格值的一部分导出。 |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | 设置导出单元格值为字符串时的格式策略。 |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | 指示是否应为空行输出分隔符。 |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | 用于在轻量模式下保存工作簿的数据提供程序。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setQuoteType(int value)](#setQuoteType-int-) | 设置在导出文本文件中如何引用值。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否缓存图表的最新数据。 |
| [setSeparator(char value)](#setSeparator-char-) | 设置文本文件的字符分隔符。 |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | 设置字符串值作为分隔符。 |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | 指示是否应像 Microsoft Excel 那样修剪前导空行和空列。 |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | 指示是否应修剪一行中尾随的空单元格。 |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | 指示是否更新 SmartArt 设置。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


创建文本文件保存选项。

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


创建文本文件保存选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat)。文件格式。它应为 [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV) 或 [SaveFormat.TSV](../../com.aspose.cells/saveformat\#TSV)，否则将自动设置保存格式为 [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV)。 |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


指示是否始终为每个字段添加 '"'。如果为 true，则所有值都会加引号；如果为 false，则仅在需要时（例如值包含特殊字符如 '"'、'\\n' 或分隔符字符）才加引号。默认值为 false。

**Remarks**

注意：此成员现已过时。请改用 QuoteType 属性。此属性将在自 2012 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

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
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


指示是否将所有工作表导出到文本文件。如果为 false，则仅导出活动工作表，类似于 MS Excel。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


要导出的单元格范围。

**Remarks**

如果已指定导出区域，则 [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) 将不起作用。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


指示当 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 为 true 时，是否应将单引号符号作为单元格值的一部分导出。默认值为 false。

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
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


指示是否应为空行输出分隔符。默认值为 false，因此默认情况下空行的内容将为空。

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


用于在轻量模式下保存工作簿的数据提供程序。

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


获取在导出文本文件中如何引用值。

参见 [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype)。

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


获取文本文件的字符分隔符。

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


获取字符串值作为分隔符。

**Returns:**
java.lang.String
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
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


指示是否应像 Microsoft Excel 那样修剪前导空行和空列。默认值为 true。

**Remarks**

与 Microsoft Excel 的规则相同，如果行/列具有自定义样式，即使不包含单元格数据，也不会被视为空白。使用 LightCells 模式保存时，此选项不起作用。用户应通过实现 [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) 或指定 [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) 来控制输出范围。

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


指示是否应修剪一行中尾随的空单元格。默认值为 false。

**Remarks**

在使用 LightCells 模式保存且未指定 [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) 时，此选项不起作用，且一行将扩展至实现 [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) 提供的最后一个单元格。

**Returns:**
boolean
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




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


指示是否始终为每个字段添加 '"'。如果为 true，则所有值都会加引号；如果为 false，则仅在需要时（例如值包含特殊字符如 '"'、'\\n' 或分隔符字符）才加引号。默认值为 false。

**Remarks**

注意：此成员现已过时。请改用 QuoteType 属性。此属性将在自 2012 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

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

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


指示是否将所有工作表导出到文本文件。如果为 false，则仅导出活动工作表，类似于 MS Excel。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


要导出的单元格范围。

**Remarks**

如果已指定导出区域，则 [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) 将不起作用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


指示当 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 为 true 时，是否应将单引号符号作为单元格值的一部分导出。默认值为 false。

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

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


指示是否应为空行输出分隔符。默认值为 false，因此默认情况下空行的内容将为空。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


用于在轻量模式下保存工作簿的数据提供程序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

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

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


设置在导出文本文件中如何引用值。

参见 [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype)。

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


设置文本文件的字符分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


设置字符串值作为分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


指示是否应像 Microsoft Excel 那样修剪前导空行和空列。默认值为 true。

**Remarks**

与 Microsoft Excel 的规则相同，如果行/列具有自定义样式，即使不包含单元格数据，也不会被视为空白。使用 LightCells 模式保存时，此选项不起作用。用户应通过实现 [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) 或指定 [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) 来控制输出范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


指示是否应修剪一行中尾随的空单元格。默认值为 false。

**Remarks**

在使用 LightCells 模式保存且未指定 [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) 时，此选项不起作用，且一行将扩展至实现 [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) 提供的最后一个单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

