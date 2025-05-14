---
title: Axis.DisplayUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the unit label for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Represents the unit label for the specified axis.

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Examples

```csharp
// Called: chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
public void Axis_Property_DisplayUnit()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;

    checkDisplayUnitType_Thousands(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkDisplayUnitType_Thousands(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkDisplayUnitType_Thousands(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


