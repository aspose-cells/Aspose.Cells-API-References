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
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56023_2.xlsx&quot;);
            workbook.Worksheets.RefreshAll();
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(&quot;=Sheet1!$G$9:$G$12&quot;, chart.NSeries[0].Values);

            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            CellArea ca = pt.RowRange;
            Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea(&quot;F9&quot;, &quot;F12&quot;), ca, &quot;PivotTable.Range&quot;));
            ca = pt.ColumnRange;
            Assert.IsTrue(CellAreaTest.equals(CellArea.CreateCellArea(&quot;G8&quot;, &quot;G8&quot;), ca, &quot;PivotTable.Range&quot;));

        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


