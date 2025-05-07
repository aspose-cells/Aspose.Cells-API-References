---
title: PivotFieldCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection property. Gets the count of the pivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/count/
---
## PivotFieldCollection.Count property

Gets the count of the pivotFields.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, pivotTable2.PageFields.Count);
[Test]
        public void Property_Count()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath  + @"CELLSNET47453.xlsx");

            var pivotTable1 = workbook.Worksheets["Sheet3"].PivotTables[0];
            var pivotTable2 = workbook.Worksheets["Sheet4"].PivotTables[0];

            var dataSource = pivotTable1.DataSource;
            // actual: null
            // expected: Sheet3!$B$2:$C$114
            Assert.AreEqual("Sheet3!$B$2:$C$114",dataSource[0]);

            var rowName = pivotTable1.RowFields[0].Name;
            // actual: [Table2].[Date].[Date]
            // expected: Date
            Assert.AreEqual("[Table2].[Date].[Date]", rowName);
           
            Assert.AreEqual(1, pivotTable2.PageFields.Count);
        }
```

### See Also

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


