---
title: PivotTable.ColumnRange
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Readonly
type: docs
url: /net/aspose.cells.pivot/pivottable/columnrange/
---
## PivotTable.ColumnRange property

Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.

```csharp
public CellArea ColumnRange { get; }
```

### Examples

```csharp
// Called: ca = pt.ColumnRange;
[Test]
        public void Property_ColumnRange()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET56023_1.xlsx");
            workbook.Worksheets.RefreshAll();
            Chart chart = workbook.Worksheets[0].Charts[0];
            
            Assert.AreEqual("=Sheet1!$G$10", chart.NSeries[0].Values);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            CellArea ca  = pt.RowRange;
            Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea("F10","F10"),ca, "PivotTable.Range"));
            ca = pt.ColumnRange;
            Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea("G8", "J9"), ca, "PivotTable.Range"));
        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


