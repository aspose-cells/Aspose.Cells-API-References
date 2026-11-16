---
title: "SettablePivotGlobalizationSettings 类"
linktitle: "SettablePivotGlobalizationSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SettablePivotGlobalizationSettings 类。封装表示 Go 中 settablepivotglobalizationsettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/settablepivotglobalizationsettings/
---

## SettablePivotGlobalizationSettings class

PivotGlobalizationSettings 的实现，支持用户设置/更改预定义文本。

```go

type SettablePivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSettablePivotGlobalizationSettings](./newsettablepivotglobalizationsettings/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetTextOfTotal](./gettextoftotal/) | 获取 PivotTable 中 "Total" 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotField 时，需要重写此方法。 |
| [SetTextOfTotal](./settextoftotal/) | 设置 PivotTable 中 "Total" 标签的文本。 |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | 获取 PivotTable 中 "Grand Total" 标签的文本。 |
| [SetTextOfGrandTotal](./settextofgrandtotal/) | 设置 PivotTable 中 "Grand Total" 标签的文本。 |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | 获取 PivotTable 中 "(Multiple Items)" 标签的文本。 |
| [SetTextOfMultipleItems](./settextofmultipleitems/) | 设置 PivotTable 中 "(Multiple Items)" 标签的文本。 |
| [GetTextOfAll](./gettextofall/) | 获取 PivotTable 中 "(All)" 标签的文本。 |
| [SetTextOfAll](./settextofall/) | 设置 PivotTable 中 "(All)" 标签的文本。 |
| [GetTextOfProtectedName](./gettextofprotectedname/) | 获取指定受保护名称的文本。 |
| [SetTextOfProtectedName](./settextofprotectedname/) | 为特定受保护名称设置文本。 |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | 获取 PivotTable 中 "Column Labels" 标签的文本。 |
| [SetTextOfColumnLabels](./settextofcolumnlabels/) | 获取 PivotTable 中 "Column Labels" 标签的文本。 |
| [GetTextOfRowLabels](./gettextofrowlabels/) | 获取 PivotTable 中 "Row Labels" 标签的文本。 |
| [SetTextOfRowLabels](./settextofrowlabels/) | 设置 PivotTable 中 "Row Labels" 标签的文本。 |
| [GetTextOfEmptyData](./gettextofemptydata/) | 获取 PivotTable 中 "(blank)" 标签的文本。 |
| [SetTextOfEmptyData](./settextofemptydata/) | 设置 PivotTable 中 "(blank)" 标签的文本。 |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | 获取 PivotTable 中值区域字段标题的文本。 |
| [SetTextOfDataFieldHeader](./settextofdatafieldheader/) | 设置 PivotTable 中值区域字段标题的文本。 |
| [GetTextOfSubTotal](./gettextofsubtotal/) | 获取 PivotTable 中 PivotFieldSubtotalType 类型的文本。 |
| [SetTextOfSubTotal](./settextofsubtotal/) | 设置 PivotTable 中 PivotFieldSubtotalType 类型的文本。 |
