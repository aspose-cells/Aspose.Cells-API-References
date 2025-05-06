---
title: PivotFilter.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Gets the name of the pivot filter
type: docs
url: /net/aspose.cells.pivot/pivotfilter/name/
---
## PivotFilter.Name property

Gets the name of the pivot filter.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sourceFilter.Name, resultFilter.Name);
[Test]
        public void Property_Name()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;CELLSAPP2228_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;input.xlsx&quot;);
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
            book.Save(savePath + &quot;out.xlsx&quot;);
            
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


