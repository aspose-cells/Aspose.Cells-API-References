---
title: DataSorter.SortLeftToRight
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false
type: docs
url: /net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Examples

```csharp
// Called: wb.DataSorter.SortLeftToRight = true;
[Test]
        public void Property_SortLeftToRight()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Sort/CellsNet45249.xlsx");

            wb.CalculateFormula();

            wb.DataSorter.Order1 = SortOrder.Ascending;
            wb.DataSorter.SortLeftToRight = true;

            Worksheet ws = wb.Worksheets["Output"];

            CellArea ca = CellArea.CreateCellArea("T1", "AK5000");

            wb.DataSorter.Key1 = 12;
            wb.DataSorter.Sort(ws.Cells, ca);
            Assert.AreEqual(ws.Cells["Y1"].Formula, "=Y4");
            wb.Save(Constants.destPath + "CellsNet45249.xlsx");
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


