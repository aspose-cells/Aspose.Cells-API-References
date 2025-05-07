---
title: Chart.ChartArea
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the chart area in the worksheet
type: docs
url: /net/aspose.cells.charts/chart/chartarea/
---
## Chart.ChartArea property

Gets the chart area in the worksheet.

```csharp
public ChartArea ChartArea { get; }
```

### Examples

```csharp
// Called: ChartArea chartarea = chart.ChartArea;
[Test]
        public void Property_ChartArea()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            chartarea.Area.FillFormat.FillType = FillType.Texture;
            chartarea.Area.FillFormat.Texture = TextureType.Canvas;

            checkFormatSetType_IsTextureSet(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkFormatSetType_IsTextureSet(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkFormatSetType_IsTextureSet(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [ChartArea](../../chartarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


