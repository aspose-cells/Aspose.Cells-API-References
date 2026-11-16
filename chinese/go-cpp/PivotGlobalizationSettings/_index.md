---
title: "PivotGlobalizationSettings 类"
linktitle: "PivotGlobalizationSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotGlobalizationSettings 类。封装在 Go 中表示 pivotglobalizationsettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

表示数据透视表的全局化设置。

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetTextOfTotal](./gettextoftotal/) | 获取 PivotTable 中 "Total" 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotField 时，需要重写此方法。 |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | 获取 PivotTable 中 "Grand Total" 标签的文本。 |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | 获取 PivotTable 中 "(Multiple Items)" 标签的文本。 |
| [GetTextOfAll](./gettextofall/) | 获取 PivotTable 中 "(All)" 标签的文本。 |
| [GetTextOfProtectedName](./gettextofprotectedname/) | 获取指定受保护名称的文本。 |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | 获取 PivotTable 中 "Column Labels" 标签的文本。 |
| [GetTextOfRowLabels](./gettextofrowlabels/) | 获取 PivotTable 中 "Row Labels" 标签的文本。 |
| [GetTextOfEmptyData](./gettextofemptydata/) | 获取 PivotTable 中 "(blank)" 标签的文本。 |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | 获取 PivotTable 中值区域字段标题的文本。 |
| [GetShortTextOf12Months](./getshorttextof12months/) | 获取 12 个月的所有短格式字符串。 |
| [GetTextOf24Hours](./gettextof24hours/) | 获取 24 小时的所有本地格式字符串。默认值为 12 AM、1 AM、2 AM、3 AM、4 AM、5 AM、6 AM、7 AM、8 AM、9 AM、10 AM、11 AM、12 PM、1 PM、2 PM、3 PM、4 PM、5 PM、6 PM、7 PM、8 PM、9 PM、10 PM、11 PM。 |
| [GetTextOfOr](./gettextofor/) | 获取 "or" 的所有本地格式字符串。 |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | 获取透视表天分组的数字格式。仅在按天对透视字段进行分组时使用。默认值为 "d-MMM"； |
| [GetTextOf4Quaters](./gettextof4quaters/) | 获取 4 个季度的本地文本。 |
| [GetTextOf4Quarters](./gettextof4quarters/) | 获取 4 个 Quaters 的本地文本。 |
| [GetTextOfYears](./gettextofyears/) | 获取 "Years" 的本地文本。 |
| [GetTextOfQuarters](./gettextofquarters/) | 获取 "Quarters" 的本地文本。 |
| [GetTextOfMonths](./gettextofmonths/) | 获取 "Months" 的本地文本。 |
| [GetTextOfDays](./gettextofdays/) | 获取 "Days" 的本地文本。 |
| [GetTextOfHours](./gettextofhours/) | 获取 "Hours" 的本地文本。 |
| [GetTextOfMinutes](./gettextofminutes/) | 获取 "Minutes" 的本地文本。 |
| [GetTextOfSeconds](./gettextofseconds/) | 获取 "Seconds" 的本地文本 |
| [GetTextOfRange](./gettextofrange/) | 获取 "Range" 的本地文本 |
| [GetTextOfAllPeriods](./gettextofallperiods/) | 获取 "All Periods" 的本地文本 |
| [GetTextOfSubTotal](./gettextofsubtotal/) | 获取 PivotTable 中 PivotFieldSubtotalType 类型的文本。 |
| [GetNameOfDataField](./getnameofdatafield/) | 获取数据透视字段的显示名称。默认格式为 "Sum Of Field"。 |
