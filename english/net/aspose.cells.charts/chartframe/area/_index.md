---
title: ChartFrame.Area
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets the area
type: docs
url: /net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

Gets the `area`.

```csharp
public virtual Area Area { get; }
```

### Examples

```csharp
// Called: chartarea.Area.FillFormat.Texture = TextureType.Canvas;
[Test]
        public void Property_Area()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            chartarea.Area.Formatting = FormattingType.Custom;
            chartarea.Area.FillFormat.Texture = TextureType.Canvas;

            checkFormattingType_Custom(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkFormattingType_Custom(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkFormattingType_Custom(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


