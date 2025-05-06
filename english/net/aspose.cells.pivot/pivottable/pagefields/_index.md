---
title: PivotTable.PageFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as page fields
type: docs
url: /net/aspose.cells.pivot/pivottable/pagefields/
---
## PivotTable.PageFields property

Returns a PivotFields object that are currently shown as page fields.

```csharp
public PivotFieldCollection PageFields { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, pivotTable2.PageFields.Count);
[Test]
        public void Property_PageFields()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath  + @&quot;CELLSNET47453.xlsx&quot;);

            var pivotTable1 = workbook.Worksheets[&quot;Sheet3&quot;].PivotTables[0];
            var pivotTable2 = workbook.Worksheets[&quot;Sheet4&quot;].PivotTables[0];

            var dataSource = pivotTable1.DataSource;
            // actual: null
            // expected: Sheet3!$B$2:$C$114
            Assert.AreEqual(&quot;Sheet3!$B$2:$C$114&quot;,dataSource[0]);

            var rowName = pivotTable1.RowFields[0].Name;
            // actual: [Table2].[Date].[Date]
            // expected: Date
            Assert.AreEqual(&quot;[Table2].[Date].[Date]&quot;, rowName);
           
            Assert.AreEqual(1, pivotTable2.PageFields.Count);
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


