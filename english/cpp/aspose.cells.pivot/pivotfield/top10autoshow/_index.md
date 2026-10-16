---
title: Aspose::Cells::Pivot::PivotField::Top10AutoShow method
linktitle: Top10AutoShow
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotField::Top10AutoShow method. Configures Top10 AutoShow settings for this pivot field in C++.'
type: docs
weight: 7700
url: /cpp/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField::Top10AutoShow method


Configures [Top10](../../../aspose.cells/top10/) AutoShow settings for this pivot field.

```cpp
void Aspose::Cells::Pivot::PivotField::Top10AutoShow(bool isAutoShow, bool isTop, int32_t count, int32_t rankBy)
```


| Parameter | Type | Description |
| --- | --- | --- |
| isAutoShow | bool | true to enable AutoShow; false to disable. |
| isTop | bool | If true, shows top items; false shows bottom items. |
| count | int32_t | Number of top/bottom items to display. |
| rankBy | int32_t | Index of data field used for ranking. Use -1 to rank by pivot item's own values. |
## Remarks



This method configures the [PivotFieldTop10AutoShowSettings](../../pivotfieldtop10autoshowsettings/).

XLS binary format: AutoShow ([Top10](../../../aspose.cells/top10/)) is the native and only supported option.

XLSX (OpenXML): The underlying file format supports [Top10](../../../aspose.cells/top10/) AutoShow, but Excel 2007 and later user interface only exposes this via [Top10](../../../aspose.cells/top10/) filter. If XLS compatibility is not required, it is recommended to use [Top10](../../../aspose.cells/top10/) filter instead.
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
