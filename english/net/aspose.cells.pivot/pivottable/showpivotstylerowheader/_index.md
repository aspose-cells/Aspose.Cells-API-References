---
title: PivotTable.ShowPivotStyleRowHeader
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the row header in the pivot table should have the style applied
type: docs
url: /net/aspose.cells.pivot/pivottable/showpivotstylerowheader/
---
## PivotTable.ShowPivotStyleRowHeader property

Indicates whether the row header in the pivot table should have the style applied.

```csharp
public bool ShowPivotStyleRowHeader { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.ShowPivotStyleRowHeader, wb_b.Worksheets[&amp;quot;SheetB&amp;quot;].PivotTables[&amp;quot;PivotTable1&amp;quot;].ShowPivotStyleRowHeader);
[Test]
        public void Property_ShowPivotStyleRowHeader()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43735_&quot;;
            Workbook wb_a = new Workbook(filePath + &quot;wbA.xlsx&quot;);
            Workbook wb_b = new Workbook(filePath + &quot;wbB.xlsx&quot;);
            wb_a.Combine(wb_b);
            wb_a.Save(Constants.PivotTableDestPath + &quot;NET43735.xlsx&quot;);

            Workbook wb = new Workbook(Constants.PivotTableDestPath + &quot;NET43735.xlsx&quot;);
            PivotTable pt = wb.Worksheets[&quot;SheetB&quot;].PivotTables[&quot;PivotTable1&quot;];
            Assert.AreEqual(pt.ShowPivotStyleRowStripes, wb_b.Worksheets[&quot;SheetB&quot;].PivotTables[&quot;PivotTable1&quot;].ShowPivotStyleRowStripes);
            Assert.AreEqual(pt.ShowPivotStyleColumnStripes, wb_b.Worksheets[&quot;SheetB&quot;].PivotTables[&quot;PivotTable1&quot;].ShowPivotStyleColumnStripes);
            Assert.AreEqual(pt.ShowPivotStyleRowHeader, wb_b.Worksheets[&quot;SheetB&quot;].PivotTables[&quot;PivotTable1&quot;].ShowPivotStyleRowHeader);
            Assert.AreEqual(pt.ShowPivotStyleColumnHeader, wb_b.Worksheets[&quot;SheetB&quot;].PivotTables[&quot;PivotTable1&quot;].ShowPivotStyleColumnHeader);
            Assert.AreEqual(pt.ShowPivotStyleLastColumn, wb_b.Worksheets[&quot;SheetB&quot;].PivotTables[&quot;PivotTable1&quot;].ShowPivotStyleLastColumn);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


