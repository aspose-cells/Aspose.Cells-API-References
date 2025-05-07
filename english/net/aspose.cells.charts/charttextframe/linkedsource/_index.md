---
title: ChartTextFrame.LinkedSource
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets and sets a reference to the worksheet
type: docs
url: /net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Gets and sets a reference to the worksheet.

```csharp
public virtual string LinkedSource { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=TitleSheet!$A$3", workbook.Worksheets[1].Charts[0].Title.LinkedSource);
[Test]
        public void Property_LinkedSource()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47520.xlsx");

            Cells titleSheet = workbook.Worksheets["TitleSheet"].Cells;
            CellArea cellArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };


            //It would seem that shifting the lines downwards causes the reference in the chart title to be lost
            //I tried both InsertRange overloads but the result is the same
            titleSheet.InsertRange(cellArea, 2, ShiftType.Down, true);
            //titleSheet.InsertRange(cellArea, ShiftType.Down);
            // Console.WriteLine(workbook.Worksheets[1].Charts[0].Title.LinkedSource);
            //=TitleSheet!$A$3
            Assert.AreEqual("=TitleSheet!$A$3", workbook.Worksheets[1].Charts[0].Title.LinkedSource);
            workbook.Save(Constants.destPath + "CellsNet47520.xlsx");
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


