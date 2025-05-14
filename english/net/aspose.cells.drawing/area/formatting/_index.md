---
title: Area.Formatting
second_title: Aspose.Cells for .NET API Reference
description: Area property. Represents the formatting of the area
type: docs
url: /net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Represents the formatting of the area.

```csharp
public FormattingType Formatting { get; set; }
```

### Examples

```csharp
// Called: chartarea.Area.Formatting = FormattingType.None;
public void Area_Property_Formatting()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    ChartArea chartarea = chart.ChartArea;
    chartarea.Area.Formatting = FormattingType.None;

    checkFormattingType_None(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkFormattingType_None(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkFormattingType_None(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


