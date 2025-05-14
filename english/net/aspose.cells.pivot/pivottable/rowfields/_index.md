---
title: PivotTable.RowFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as row fields
type: docs
url: /net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Returns a PivotFields object that are currently shown as row fields.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Examples

```csharp
// Called: var rowName = pivotTable1.RowFields[0].Name;
public void PivotTable_Property_RowFields()
{
    var workbook = new Workbook(Constants.PivotTableSourcePath  + @"example.xlsx");

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

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


