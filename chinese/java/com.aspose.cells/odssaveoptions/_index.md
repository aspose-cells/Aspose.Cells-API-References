---
title: "OdsSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示保存 ods 文件的选项。"
type: docs
url: /zh/java/com.aspose.cells/odssaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OdsSaveOptions extends SaveOptions
```

表示保存 ods 文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [OdsSaveOptions()](#OdsSaveOptions--) | 创建保存 ODS 文件的选项。 |
| [OdsSaveOptions(int saveFormat)](#OdsSaveOptions-int-) | 创建保存 ODS 文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | 用于临时文件的文件夹，可用作数据缓存。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [getGeneratorType()](#getGeneratorType--) | 获取 ODS 文件的生成器。 |
| [getIgnorePivotTables()](#getIgnorePivotTables--) | 指示是否保存数据透视表。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getOdfStrictVersion()](#getOdfStrictVersion--) | 获取 ODF 版本。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否缓存图表的最新数据。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSortExternalNames()](#getSortExternalNames--) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | 指示是否更新 SmartArt 设置。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hashCode()](#hashCode--) |  |
| [isStrictSchema11()](#isStrictSchema11--) | 指示 ODS 文件是否应保存为 ODF 格式版本 1.1。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 用于临时文件的文件夹，可用作数据缓存。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [setGeneratorType(int value)](#setGeneratorType-int-) | 设置 ODS 文件的生成器。 |
| [setIgnorePivotTables(boolean value)](#setIgnorePivotTables-boolean-) | 指示是否保存数据透视表。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setOdfStrictVersion(int value)](#setOdfStrictVersion-int-) | 设置 ODF 版本。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否缓存图表的最新数据。 |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setStrictSchema11(boolean value)](#setStrictSchema11-boolean-) | 指示 ODS 文件是否应保存为 ODF 格式版本 1.1。 |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | 指示是否更新 SmartArt 设置。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OdsSaveOptions() {#OdsSaveOptions--}
```
public OdsSaveOptions()
```


创建保存 ODS 文件的选项。

### OdsSaveOptions(int saveFormat) {#OdsSaveOptions-int-}
```
public OdsSaveOptions(int saveFormat)
```


创建保存 ODS 文件的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat)。文件格式。它应该是 [SaveFormat.ODS](../../com.aspose.cells/saveformat\#ODS)、[SaveFormat.OTS](../../com.aspose.cells/saveformat\#OTS)、[SaveFormat.FODS](../../com.aspose.cells/saveformat\#FODS) 或 [SaveFormat.SXC](../../com.aspose.cells/saveformat\#SXC)，否则保存的格式将自动设置为 [SaveFormat.ODS](../../com.aspose.cells/saveformat\#ODS)。 |

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
### getGeneratorType() {#getGeneratorType--}
```
public int getGeneratorType()
```


获取 ODS 文件的生成器。

参见 [OdsGeneratorType](../../com.aspose.cells/odsgeneratortype)。

**Returns:**
int
### getIgnorePivotTables() {#getIgnorePivotTables--}
```
public boolean getIgnorePivotTables()
```


指示是否保存数据透视表。

**Remarks**

OpenOffice 的数据透视表功能相比 Excel 设置较少，因此它们的数据透视表结果有许多差异。有时在保存 .ods 文件时最好忽略这些数据透视表。

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
### getOdfStrictVersion() {#getOdfStrictVersion--}
```
public int getOdfStrictVersion()
```


获取 ODF 版本。

参见 [OpenDocumentFormatVersionType](../../com.aspose.cells/opendocumentformatversiontype)。

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
### isStrictSchema11() {#isStrictSchema11--}
```
public boolean isStrictSchema11()
```


指示是否将 ods 文件保存为 ODF 格式版本 1.1。默认值为 false。

**Remarks**

注意：此成员已过时。请改用 OdsSaveOptions.OdfStrictVersion 属性。此方法将在自 2024 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

### setGeneratorType(int value) {#setGeneratorType-int-}
```
public void setGeneratorType(int value)
```


设置 ODS 文件的生成器。

参见 [OdsGeneratorType](../../com.aspose.cells/odsgeneratortype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIgnorePivotTables(boolean value) {#setIgnorePivotTables-boolean-}
```
public void setIgnorePivotTables(boolean value)
```


指示是否保存数据透视表。

**Remarks**

OpenOffice 的数据透视表功能相比 Excel 设置较少，因此它们的数据透视表结果有许多差异。有时在保存 .ods 文件时最好忽略这些数据透视表。

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

### setOdfStrictVersion(int value) {#setOdfStrictVersion-int-}
```
public void setOdfStrictVersion(int value)
```


设置 ODF 版本。

参见 [OpenDocumentFormatVersionType](../../com.aspose.cells/opendocumentformatversiontype)。

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

### setStrictSchema11(boolean value) {#setStrictSchema11-boolean-}
```
public void setStrictSchema11(boolean value)
```


指示是否将 ods 文件保存为 ODF 格式版本 1.1。默认值为 false。

**Remarks**

注意：此成员已过时。请改用 OdsSaveOptions.OdfStrictVersion 属性。此方法将在自 2024 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

