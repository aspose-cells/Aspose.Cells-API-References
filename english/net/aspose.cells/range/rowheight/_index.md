---
title: Range.RowHeight
second_title: Aspose.Cells for .NET API Reference
description: Range property. Sets or gets the height of rows in this range
type: docs
url: /net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Sets or gets the height of rows in this range

```csharp
public double RowHeight { get; set; }
```

### Examples

```csharp
// Called: Height = sourceWorkbook.Worksheets[0].Cells.CreateRange("1:1").RowHeight;
[Test]
        public void Property_RowHeight()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath +  "CellsNet42476.xlsx");
            AutoFitterOptions oAutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true, IgnoreHidden = true, OnlyAuto = false };
            double Height = sourceWorkbook.Worksheets[0].Cells.CreateRange("1:1").RowHeight;
            sourceWorkbook.Worksheets[0].AutoFitRow(0, 0, 16383, oAutoFitterOptions);
            Height = sourceWorkbook.Worksheets[0].Cells.CreateRange("1:1").RowHeight;
            Assert.AreEqual(Height, 15.75);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


