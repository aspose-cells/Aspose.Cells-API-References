---
title: PivotTable.PivotFilters
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns all filters of pivot fields in the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Returns all filters of pivot fields in the pivot table.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Examples

```csharp
// Called: PivotFilter sourceFilter = wb.Worksheets[0].PivotTables[0].PivotFilters[0];
[Test]
        public void Property_PivotFilters()
        {
            string filePath = Constants.PivotTableSourcePath + @"CELLSAPP2228_";
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + "input.xlsx");
            PivotFilter sourceFilter = wb.Worksheets[0].PivotTables[0].PivotFilters[0];
            Workbook book = new Workbook();
            book.Copy(wb);
            PivotFilter resultFilter = book.Worksheets[0].PivotTables[0].PivotFilters[0];
            Assert.AreEqual(sourceFilter.Name, resultFilter.Name);
            Assert.AreEqual(sourceFilter.Value1, resultFilter.Value1);
            Assert.AreEqual(sourceFilter.Value2, resultFilter.Value2);
            Assert.AreEqual(sourceFilter.FieldIndex, resultFilter.FieldIndex);
            Assert.AreEqual(sourceFilter.ValueFieldIndex, resultFilter.ValueFieldIndex);
            Assert.AreEqual(sourceFilter.FilterType, resultFilter.FilterType);

           // Assert.AreEqual(sourceFilter.AutoFilter.Range, resultFilter.AutoFilter.Range);
          //  Assert.AreEqual(sourceFilter.AutoFilter.FilterColumns.Count, resultFilter.AutoFilter.FilterColumns.Count);
            book.Save(savePath + "out.xlsx");
            
        }
```

### See Also

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


