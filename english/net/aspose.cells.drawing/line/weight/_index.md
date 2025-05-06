---
title: Line.Weight
second_title: Aspose.Cells for .NET API Reference
description: Line property. Gets or sets the WeightType of the line
type: docs
url: /net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

Gets or sets the [`WeightType`](../../weighttype/) of the line.

```csharp
public WeightType Weight { get; set; }
```

### Examples

```csharp
// Called: chartarea.Border.Weight = WeightType.MediumLine;
[Test]
        public void Property_Weight()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            chartarea.Border.Weight = WeightType.MediumLine;

            checkWeightType_MediumLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkWeightType_MediumLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkWeightType_MediumLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


