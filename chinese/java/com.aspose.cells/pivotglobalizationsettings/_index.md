---
title: "PivotGlobalizationSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视表的全球化设置。"
type: docs
url: /zh/java/com.aspose.cells/pivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotGlobalizationSettings
```

表示数据透视表的全球化设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotGlobalizationSettings()](#PivotGlobalizationSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | 获取透视表日期组的数字格式。 |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | 获取数据透视字段的显示名称。 |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | 获取 12 个月的所有简短格式字符串。 |
| [getTextOf24Hours()](#getTextOf24Hours--) | 获取 24 小时的所有本地格式字符串。 |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | 获取 4 个季度的本地文本。 |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | 获取 4 个季度的本地文本。 |
| [getTextOfAll()](#getTextOfAll--) | 获取透视表中 "(All)" 标签的文本。 |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | 获取 "All Periods" 的本地化文本。 |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | 获取透视表中 "Column Labels" 标签的文本。 |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | 获取 PivotTable 中值区域字段标题的文本。 |
| [getTextOfDays()](#getTextOfDays--) | 获取 "Days" 的本地文本。 |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | 获取 PivotTable 中 "(blank)" 标签的文本。 |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | 获取 PivotTable 中 "Grand Total" 标签的文本。 |
| [getTextOfHours()](#getTextOfHours--) | 获取 "Hours" 的本地文本。 |
| [getTextOfMinutes()](#getTextOfMinutes--) | 获取 "Minutes" 的本地文本。 |
| [getTextOfMonths()](#getTextOfMonths--) | 获取 "Months" 的本地文本。 |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | 获取 PivotTable 中 "(Multiple Items)" 标签的文本。 |
| [getTextOfOr()](#getTextOfOr--) | 获取 "or" 的所有本地格式化字符串。 |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | 获取指定受保护名称的文本。 |
| [getTextOfProtection()](#getTextOfProtection--) | 获取透视表中的保护名称。 |
| [getTextOfQuarters()](#getTextOfQuarters--) | 获取 "Quarters" 的本地文本。 |
| [getTextOfRange()](#getTextOfRange--) | 获取 "Range" 的本地文本 |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | 获取 PivotTable 中 "Row Labels" 标签的文本。 |
| [getTextOfSeconds()](#getTextOfSeconds--) | 获取 "Seconds" 的本地文本 |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | 获取 PivotTable 中 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) 类型的文本。 |
| [getTextOfTotal()](#getTextOfTotal--) | 获取 PivotTable 中 "Total" 标签的文本。 |
| [getTextOfYears()](#getTextOfYears--) | 获取 "Years" 的本地文本。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotGlobalizationSettings() {#PivotGlobalizationSettings--}
```
public PivotGlobalizationSettings()
```


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
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


获取透视表日期分组的数字格式。仅在按天对透视字段进行分组时使用。默认值为 "d-MMM"；

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


获取数据透视字段的显示名称。默认格式为 "Sum Of Field"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。该函数用于汇总透视字段的值。 |
| 名称 | java.lang.String | 透视字段的原始名称。 |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


获取 12 个月的所有简短格式字符串。

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


获取 24 小时的所有本地格式化字符串。默认值为 12 AM、1 AM、2 AM、3 AM、4 AM、5 AM、6 AM、7 AM、8 AM、9 AM、10 AM、11 AM、12 PM、1 PM、2 PM、3 PM、4 PM、5 PM、6 PM、7 PM、8 PM、9 PM、10 PM、11 PM。

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


获取 4 个季度的本地文本。

**Remarks**

在 26.9 之前默认返回 Quarter1、Quarter2、Quarter3、Quarter4。自 26.9 起默认返回 Qtr1、Qtr2、Qtr3、Qtr4。

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


获取 4 个季度的本地文本。

**Remarks**

注意：此成员已过时。请改用 PivotGlobalizationSettings.GetTextOf4Quarters() 方法。此属性将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


获取透视表中 "(All)" 标签的文本。

**Returns:**
java.lang.String - "(All)" 标签的文本
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


获取 "All Periods" 的本地化文本。

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


获取透视表中 "Column Labels" 标签的文本。

**Returns:**
java.lang.String - 列标签的文本
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


获取 PivotTable 中值区域字段标题的文本。

**Returns:**
java.lang.String - 数据字段标题名称的文本
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


获取 "Days" 的本地文本。

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


获取 PivotTable 中 "(blank)" 标签的文本。

**Returns:**
java.lang.String - 空数据的文本
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


获取 PivotTable 中 "Grand Total" 标签的文本。

**Returns:**
java.lang.String - "Grand Total" 标签的文本
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


获取 "Hours" 的本地文本。

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


获取 "Minutes" 的本地文本。

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


获取 "Months" 的本地文本。

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


获取 PivotTable 中 "(Multiple Items)" 标签的文本。

**Returns:**
java.lang.String - "(Multiple Items)" 标签的文本
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


获取 "or" 的所有本地格式化字符串。

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


获取指定受保护名称的文本。

**Remarks**

在 Microsoft Excel 中，某些名称不能用作 PivotTable 中 PivotFields 的名称。它们因地区而异，用户可以根据所使用的地区显式指定这些名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| protectedName | java.lang.String | PivotTable 中的受保护名称。 |

**Returns:**
java.lang.String - PivotTable 的本地受保护名称。
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


获取透视表中的保护名称。

**Remarks**

注意：此成员已过时。请改用 PivotGlobalizationSettings.GetTextOfProtectedName(string) 方法。此属性将在自 2023 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String - PivotTable 的保护名称
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


获取 "Quarters" 的本地文本。

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


获取 "Range" 的本地文本

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


获取 PivotTable 中 "Row Labels" 标签的文本。

**Returns:**
java.lang.String - 行标签的文本
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


获取 "Seconds" 的本地文本

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


获取 PivotTable 中 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) 类型的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。该 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - 给定类型的文本
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


获取 PivotTable 中 "Total" 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotFields 时，需要重写此方法。

**Returns:**
java.lang.String - "Total" 标签的文本
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


获取 "Years" 的本地文本。

**Returns:**
java.lang.String -
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

