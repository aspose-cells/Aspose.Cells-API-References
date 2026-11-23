---
title: "PivotField.Top10AutoShow"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。为此透视字段配置 Top10 AutoShow 设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

为此透视字段配置 Top10 AutoShow 设置。

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAutoShow | 布尔 | true 表示启用 AutoShow；false 表示禁用。 |
| isTop | 布尔 | 如果为 true，则显示顶部项目；如果为 false，则显示底部项目。 |
| 计数 | Int32 | 要显示的顶部/底部项目数量。 |
| rankBy | Int32 | 用于排名的数据字段索引。使用 -1 以按透视项自身的值进行排名。 |

### 备注

此方法配置 [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/)。

XLS 二进制格式：AutoShow（Top10）是原生且唯一支持的选项。

XLSX（OpenXML）：底层文件格式支持 Top10 AutoShow，但 Excel 2007 及更高版本的用户界面仅通过 Top10 筛选器公开此功能。如果不需要 XLS 兼容性，建议改用 Top10 筛选器。

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


