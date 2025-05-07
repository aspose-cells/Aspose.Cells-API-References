---
title: Range.FirstColumn
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the index of the first column of the range
type: docs
url: /net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Gets the index of the first column of the range.

```csharp
public int FirstColumn { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(6, ra.FirstColumn, ra.ColumnCount- 1);
[Test]
        public void Property_FirstColumn()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET53416.xlsx");
            var worksheet = wb.Worksheets["国债期货"];
            // worksheet.Cells.ClearMergedCells();
            worksheet.RefreshPivotTables();
            wb.Save(Constants.PivotTableDestPath + "CELLSNET53416.xlsx");
            Aspose.Cells.Range ra = worksheet.Cells["E3"].GetMergedRange();
            Assert.AreEqual(6, ra.FirstColumn, ra.ColumnCount- 1);
            Assert.AreEqual(2, ra.FirstRow);
            Assert.IsTrue(worksheet.Cells["A5"].StringValue.StartsWith("CDB10"));//CELLSNET-57346

        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


