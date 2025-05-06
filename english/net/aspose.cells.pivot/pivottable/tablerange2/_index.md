---
title: PivotTable.TableRange2
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a CellArea object that represents the range containing the entire PivotTable report includes page fields. Readonly
type: docs
url: /net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.

```csharp
public CellArea TableRange2 { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(10, pt.TableRange2.EndRow);
[Test]
        public void Property_TableRange2()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + @&quot;CELLSNET56909.xls&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET56909.ods&quot;);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET56909.ods&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            Assert.AreEqual(10, pt.TableRange2.EndRow);
            Assert.AreEqual(ConsolidationFunction.Count, pt.DataFields[0].Function);
            workbook.Worksheets.RefreshAll();
            Assert.AreEqual(&quot;Count of b&quot;, workbook.Worksheets[0].Cells[&quot;F8&quot;].StringValue);
          
        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


