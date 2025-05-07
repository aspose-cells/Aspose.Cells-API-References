---
title: SparklineGroup.PlotEmptyCellsType
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Indicates how to plot empty cells
type: docs
url: /net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Indicates how to plot empty cells.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
[Test]
        public void Property_PlotEmptyCellsType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET58096.xlsx");

            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the first sparkline group
            SparklineGroup group = worksheet.SparklineGroups[0];

            // Add Data Ranges and Locations inside this sparkline group
            int index = group.Sparklines.Add("D5:O5", 4, 15);
            Assert.AreEqual("Sheet1!D5:O5", group.Sparklines[index].DataRange);
            //group.Sparklines.Add("D6:O6", 5, 15);
            //group.Sparklines.Add("D7:O7", 6, 15);
            //group.Sparklines.Add("D8:O8", 7, 15);

            // Save the workbook
            workbook.Save(Constants.destPath + "CELLSNET58096.xlsb");
            workbook = new Workbook(Constants.destPath + "CELLSNET58096.xlsb");
            group = worksheet.SparklineGroups[0];
            Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
            workbook.Save(Constants.destPath + "CELLSNET58096.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET58096.xlsx");
            group = worksheet.SparklineGroups[0];
            Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
        }
```

### See Also

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


