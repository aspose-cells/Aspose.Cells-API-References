---
title: "GlobalizationSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示全局化设置。"
type: docs
url: /zh/java/com.aspose.cells/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

表示全局化设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | 根据特定的排序规则比较两个字符串值。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | 获取 PivotTable 中 "(All)" 标签的名称。 |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | 获取单元格布尔值的显示字符串。 |
| [getChartSettings()](#getChartSettings--) | 获取图表的全局化设置。 |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | 根据特定的排序规则将字符串转换为可比较的对象。 |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | 获取 PivotTable 中 "Column Labels" 标签的名称。 |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | 获取公式中数组行数据项的分隔符。 |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | 根据评论标题类型获取与区域设置相关的评论标题名称。 |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | 获取 PivotTable 中值区域字段标题的名称。 |
| [getDefaultSheetName()](#getDefaultSheetName--) | 获取自动添加工作表时的默认工作表名称。 |
| [getEmptyDataName()](#getEmptyDataName--) | 获取透视表中 "(blank)" 标签的名称。 |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | 获取单元格错误值的显示字符串 |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | 获取函数的总计名称。 |
| [getListSeparator()](#getListSeparator--) | 获取列表、函数参数等的分隔符。 |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | 根据给定的标准文本获取内置名称的区域性相关文本。 |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | 根据给定的标准函数名称获取区域性相关的函数名称。 |
| [getMultipleItemsName()](#getMultipleItemsName--) | 获取透视表中 "(Multiple Items)" 标签的名称。 |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | 获取透视表中 "Grand Total" 标签的名称。 |
| [getPivotSettings()](#getPivotSettings--) | 获取透视表的全球化设置。 |
| [getPivotTotalName()](#getPivotTotalName--) | 获取透视表中 "Total" 标签的名称。 |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | 获取透视表中的保护名称。 |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | 获取透视表中 "Row Labels" 标签的名称。 |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | 获取公式中数组数据行的分隔符。 |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | 根据给定的区域性相关文本获取内置名称的标准文本。 |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | 根据给定的区域性相关函数名称获取标准函数名称。 |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | 根据给定的区域性字体样式名称获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。 |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | 获取透视表中 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) 类型的名称。 |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | 获取引用表中所有行组成的表行类型名称。 |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | 获取引用表中当前行组成的表行类型名称。 |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | 获取引用表中数据区域组成的表行类型名称。 |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | 获取表头组成的表行类型名称。 |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | 获取引用表中总计行组成的表行类型名称。 |
| [getTotalName(int functionType)](#getTotalName-int-) | 获取函数的完整名称。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | 设置图表的全球化设置。 |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | 设置数据透视表的全局化设置。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


根据特定的排序规则比较两个字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| v1 | java.lang.String | 第一个字符串 |
| v2 | java.lang.String | 第二个字符串 |
| ignoreCase | boolean | 比较值时是否忽略大小写 |

**Returns:**
int - 表示两个比较对象之间词法关系的整数
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


获取 PivotTable 中 "(All)" 标签的名称。

**Remarks**

注意：此成员已过时。请改用 GlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。该属性将在自2022年12月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String - “(All)” 标签的名称
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


获取单元格布尔值的显示字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| bv | boolean | 布尔值 |

**Returns:**
java.lang.String - 默认返回 "TRUE" 表示真值，返回 "FALSE" 表示假值。
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


获取图表的全局化设置。

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


根据特定的排序规则将字符串转换为可比较的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| v | java.lang.String | 字符串值需要与其他值进行比较。 |
| ignoreCase | boolean | 比较值时是否忽略大小写 |

**Returns:**
java.lang.Comparable - 对象可用于比较或排序字符串值
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


获取 PivotTable 中 "Column Labels" 标签的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - 列标签的名称
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


获取公式中数组行数据项的分隔符。

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


根据评论标题类型获取与区域设置相关的评论标题名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). |

**Returns:**
java.lang.String -
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


获取 PivotTable 中值区域字段标题的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - 数据字段标题的名称
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


获取自动添加工作表时的默认工作表名称。默认值为 "Sheet"。

**Remarks**

自动添加的工作表（例如通过 [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\\#add--)）的名称将是指定名称加上序号。例如，德国用户可能希望工作表名称为 "Tabellenblatt2" 而不是 "Sheet2"。此时用户可以实现此方法返回 "Tabellenblatt"。

**Returns:**
java.lang.String - 自动添加工作表时的默认工作表名称
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


获取透视表中 "(blank)" 标签的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - 空数据的名称
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


获取单元格错误值的显示字符串

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| err | java.lang.String | 错误值，例如 \\#VALUE!、\\#NAME? |

**Returns:**
java.lang.String - 默认返回错误值本身
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


获取函数的总计名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。函数类型。 |

**Returns:**
java.lang.String - 函数的总计名称
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


获取列表、函数参数等的分隔符。

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


根据给定的标准文本获取内置名称的区域性相关文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| standardName | java.lang.String | Standard（en-US 区域）内置名称的文本。 |

**Returns:**
java.lang.String - 区域相关的文本。该区域由使用此设置的工作簿指定。
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


根据给定的标准函数名称获取区域性相关的函数名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| standardName | java.lang.String | Standard（en-US 区域）函数名称。 |

**Returns:**
java.lang.String - 区域相关的函数名称。该区域由使用此设置的工作簿指定。
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


获取透视表中 "(Multiple Items)" 标签的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - "(Multiple Items)" 标签的名称
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


获取透视表中 "Grand Total" 标签的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - "Grand Total" 标签的名称
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


获取透视表的全球化设置。

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


获取 PivotTable 中 "Total" 标签的名称。当 PivotTable 在数据区域包含两个或更多 PivotFields 时，需要重写此方法。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - "Total" 标签的名称
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


获取透视表中的保护名称。

**Remarks**

注意：此成员已过时。请改用 PivotGlobalizationSettings.GetTextOfProtectedName(string) 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String - PivotTable 的保护名称
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


获取透视表中 "Row Labels" 标签的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.lang.String - 行标签的名称
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


获取公式中数组数据行的分隔符。

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


根据给定的区域性相关文本获取内置名称的标准文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localName | java.lang.String | 基于区域设置的内置名称文本。该区域设置由使用此设置的 Workbook 指定。 |

**Returns:**
java.lang.String - 标准（en-US 区域设置）文本。
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


根据给定的区域性相关函数名称获取标准函数名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localName | java.lang.String | 基于区域设置的函数名称。该区域设置由使用此设置的 Workbook 指定。 |

**Returns:**
java.lang.String - 标准（en-US 区域设置）函数名称。
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


根据给定的区域性字体样式名称获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Header/Footer 的区域设置字体样式名称。 |

**Returns:**
java.lang.String - 标准英文字体样式名称（Regular，Bold，Italic）
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


获取透视表中 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) 类型的名称。

**Remarks**

注意：此成员现已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年12月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。[PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) 类型 |

**Returns:**
java.lang.String - [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) 类型的名称
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


获取引用表中所有行组成的表行类型名称。默认值为 "All"，因此在公式 "\#All" 中表示引用表的所有行。

**Returns:**
java.lang.String - 表行的类型名称
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


获取引用表中由当前行组成的表行的类型名称。默认是 "This Row"，因此在公式 "\#This Row" 中表示引用表中的当前行。

**Returns:**
java.lang.String - 表行的类型名称
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


获取由引用表的数据区域组成的表行的类型名称。默认值为 "Data"，因此在公式 "\#Data" 中表示表的数据区域。

**Returns:**
java.lang.String - 表行的类型名称
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


获取由表头组成的表行的类型名称。默认值为 "Headers"，因此在公式 "\#Headers" 中表示表头。

**Returns:**
java.lang.String - 表行的类型名称
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


获取引用表中由总计行组成的表行的类型名称。默认是 "Totals"，因此在公式 "\#Totals" 中表示引用表中的总计行。

**Returns:**
java.lang.String - 表行的类型名称
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


获取函数的完整名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。函数类型。 |

**Returns:**
java.lang.String - 函数的总名称
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




### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


设置图表的全球化设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


设置数据透视表的全局化设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

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

