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
// Called: CellArea ca  = pt.RowRange;
[Test]
        public void Property_RowRange()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56023_1.xlsx&quot;);
            workbook.Worksheets.RefreshAll();
            Chart chart = workbook.Worksheets[0].Charts[0];
            
            Assert.AreEqual(&quot;=Sheet1!$G$10&quot;, chart.NSeries[0].Values);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            CellArea ca  = pt.RowRange;
            Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea(&quot;F10&quot;,&quot;F10&quot;),ca, &quot;PivotTable.Range&quot;));
            ca = pt.ColumnRange;
            Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea(&quot;G8&quot;, &quot;J9&quot;), ca, &quot;PivotTable.Range&quot;));
        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


