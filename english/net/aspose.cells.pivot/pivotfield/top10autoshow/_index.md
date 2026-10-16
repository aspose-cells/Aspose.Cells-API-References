---
title: PivotField.Top10AutoShow
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Configures Top10 AutoShow settings for this pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Configures Top10 AutoShow settings for this pivot field.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isAutoShow | Boolean | true to enable AutoShow; false to disable. |
| isTop | Boolean | If true, shows top items; false shows bottom items. |
| count | Int32 | Number of top/bottom items to display. |
| rankBy | Int32 | Index of data field used for ranking. Use -1 to rank by pivot item's own values. |

### Remarks

This method configures the [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

XLS binary format: AutoShow (Top10) is the native and only supported option.

XLSX (OpenXML): The underlying file format supports Top10 AutoShow, but Excel 2007 and later user interface only exposes this via Top10 filter. If XLS compatibility is not required, it is recommended to use Top10 filter instead.

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


