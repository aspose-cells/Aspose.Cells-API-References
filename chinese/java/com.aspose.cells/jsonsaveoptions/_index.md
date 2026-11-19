---
title: "JsonSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示将工作簿保存为 JSON 文件的选项。"
type: docs
url: /zh/java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

表示将工作簿保存为 JSON 文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | 创建用于保存 JSON 文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--) | 指示是否始终将 Excel 导出为 JSON 对象，即使文件中只有一个工作表。 |
| [getCachedFileFolder()](#getCachedFileFolder--) | 用于临时文件的文件夹，可用作数据缓存。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [getExportArea()](#getExportArea--) | 获取导出范围。 |
| [getExportAsString()](#getExportAsString--) | 将单元格的字符串值导出为 JSON。 |
| [getExportEmptyCells()](#getExportEmptyCells--) | 指示是否将空单元格导出为 null。 |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | 表示导出超链接到 JSON 的类型。 |
| [getExportNestedStructure()](#getExportNestedStructure--) | 导出为父子层级的 JSON 结构。 |
| [getExportStylePool()](#getExportStylePool--) | 指示是将样式整体导出还是分别导出到每个单元格。 |
| [getIndent()](#getIndent--) | 指示缩进。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否缓存图表的最新数据。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSchemas()](#getSchemas--) | 每个工作表的原始 JSON 架构。 |
| [getSheetIndexes()](#getSheetIndexes--) | 表示已导出工作表的索引。 |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | 指示是否跳过空行。 |
| [getSortExternalNames()](#getSortExternalNames--) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getToExcelStruct()](#getToExcelStruct--) | 指示是否将 Excel 文件转换为 json 结构。 |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | 指示是否更新 SmartArt 设置。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hasHeaderRow()](#hasHeaderRow--) | 指示范围是否包含标题行。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysExportAsJsonObject(boolean value)](#setAlwaysExportAsJsonObject-boolean-) | 指示是否始终将 Excel 导出为 JSON 对象，即使文件中只有一个工作表。 |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 用于临时文件的文件夹，可用作数据缓存。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | 设置导出范围。 |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | 将单元格的字符串值导出为 JSON。 |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | 指示是否将空单元格导出为 null。 |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | 表示导出超链接到 JSON 的类型。 |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | 导出为父子层级的 JSON 结构。 |
| [setExportStylePool(boolean value)](#setExportStylePool-boolean-) | 指示是将样式整体导出还是分别导出到每个单元格。 |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | 指示范围是否包含标题行。 |
| [setIndent(String value)](#setIndent-java.lang.String-) | 指示缩进。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否缓存图表的最新数据。 |
| [setSchemas(String[] value)](#setSchemas-java.lang.String---) | 每个工作表的原始 JSON 架构。 |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | 表示已导出工作表的索引。 |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | 指示是否跳过空行。 |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setToExcelStruct(boolean value)](#setToExcelStruct-boolean-) | 指示是否将 Excel 文件转换为 json 结构。 |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | 指示是否更新 SmartArt 设置。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonSaveOptions() {#JsonSaveOptions--}
```
public JsonSaveOptions()
```


创建用于保存 JSON 文件的选项。

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
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```
public boolean getAlwaysExportAsJsonObject()
```


指示是否始终将 Excel 导出为 JSON 对象，即使文件中只有一个工作表。

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
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

**Remarks**

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


获取导出范围。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


将单元格的字符串值导出为 JSON。

**Returns:**
boolean
### getExportEmptyCells() {#getExportEmptyCells--}
```
public boolean getExportEmptyCells()
```


指示是否将空单元格导出为 null。

**Returns:**
boolean
### getExportHyperlinkType() {#getExportHyperlinkType--}
```
public int getExportHyperlinkType()
```


表示导出超链接到 JSON 的类型。

参见 [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype)。

**Remarks**

默认值是 [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING)；

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


导出为父子层级的 JSON 结构。

**Remarks**

**Returns:**
boolean
### getExportStylePool() {#getExportStylePool--}
```
public boolean getExportStylePool()
```


指示是将样式整体导出还是分别导出到每个单元格。

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


指示缩进。

**Remarks**

如果缩进为 null 或为空，则导出的 json 不会进行格式化。

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
### getSchemas() {#getSchemas--}
```
public String[] getSchemas()
```


每个工作表的原始 JSON 架构。

**Returns:**
java.lang.String[]
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


表示已导出工作表的索引。

**Returns:**
int[]
### getSkipEmptyRows() {#getSkipEmptyRows--}
```
public boolean getSkipEmptyRows()
```


指示是否跳过空行。

**Returns:**
boolean
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
### getToExcelStruct() {#getToExcelStruct--}
```
public boolean getToExcelStruct()
```


指示是否将 Excel 文件转换为 json 结构。

**Remarks**

仅用于将范围转换为 JSON。

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
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


指示范围是否包含标题行。

**Returns:**
boolean
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




### setAlwaysExportAsJsonObject(boolean value) {#setAlwaysExportAsJsonObject-boolean-}
```
public void setAlwaysExportAsJsonObject(boolean value)
```


指示是否始终将 Excel 导出为 JSON 对象，即使文件中只有一个工作表。

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

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


设置导出范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


将单元格的字符串值导出为 JSON。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


指示是否将空单元格导出为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


表示导出超链接到 JSON 的类型。

参见 [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype)。

**Remarks**

默认值是 [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING)；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


导出为父子层级的 JSON 结构。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportStylePool(boolean value) {#setExportStylePool-boolean-}
```
public void setExportStylePool(boolean value)
```


指示是将样式整体导出还是分别导出到每个单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


指示范围是否包含标题行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


指示缩进。

**Remarks**

如果缩进为 null 或为空，则导出的 json 不会进行格式化。

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


指示是否缓存图表的最新数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSchemas(String[] value) {#setSchemas-java.lang.String---}
```
public void setSchemas(String[] value)
```


每个工作表的原始 JSON 架构。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String[] |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


表示已导出工作表的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


指示是否跳过空行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

### setToExcelStruct(boolean value) {#setToExcelStruct-boolean-}
```
public void setToExcelStruct(boolean value)
```


指示是否将 Excel 文件转换为 json 结构。

**Remarks**

仅用于将范围转换为 JSON。

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

