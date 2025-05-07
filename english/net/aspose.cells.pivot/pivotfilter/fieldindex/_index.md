---
title: PivotFilter.FieldIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Gets the index of source field which this pivot filter is applied to
type: docs
url: /net/aspose.cells.pivot/pivotfilter/fieldindex/
---
## PivotFilter.FieldIndex property

Gets the index of source field which this pivot filter is applied to.

```csharp
public int FieldIndex { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sourceFilter.FieldIndex, resultFilter.FieldIndex);
[Test]
        public void Property_FieldIndex()
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

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


