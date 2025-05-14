---
title: PivotTable.RowRange
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Readonly
type: docs
url: /net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.

```csharp
public CellArea RowRange { get; }
```

### Examples

```csharp
// Called: CellArea ca = pt.RowRange;
public void PivotTable_Property_RowRange()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets.RefreshAll();
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual("=Sheet1!$G$9:$G$12", chart.NSeries[0].Values);

    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    CellArea ca = pt.RowRange;
    Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea("F9", "F12"), ca, "PivotTable.Range"));
    ca = pt.ColumnRange;
    Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea("G8", "G8"), ca, "PivotTable.Range"));

}
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


