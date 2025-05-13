---
title: ErrorBar.DisplayType
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents the display type of error bar
type: docs
url: /net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Represents the display type of error bar.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;
public void ErrorBar_Property_DisplayType()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;

    checkErrorBarDisplayType_Plus(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkErrorBarDisplayType_Plus(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkErrorBarDisplayType_Plus(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


