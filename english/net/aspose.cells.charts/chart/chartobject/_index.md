---
title: Chart.ChartObject
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Represents the chartShape
type: docs
url: /net/aspose.cells.charts/chart/chartobject/
---
## Chart.ChartObject property

Represents the chartShape;

```csharp
public ChartShape ChartObject { get; }
```

### Examples

```csharp
// Called: chart.ChartObject.Placement = PlacementType.Move;
public void Chart_Property_ChartObject()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.ChartObject.Placement = PlacementType.Move;

    checkPlacementType_Move(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkPlacementType_Move(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkPlacementType_Move(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [ChartShape](../../../aspose.cells.drawing/chartshape/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


