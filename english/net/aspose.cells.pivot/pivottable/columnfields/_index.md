---
title: PivotTable.ColumnFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as column fields
type: docs
url: /net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Returns a PivotFields object that are currently shown as column fields.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Examples

```csharp
// Called: PivotField field = pivot.ColumnFields[0];
public void PivotTable_Property_ColumnFields() 
{
    Workbook book = AddNewWorkbok();
    PivotTable pivot = AddNewPivotTable(book);
    //Add PivotFilter
    PivotField field = pivot.ColumnFields[0];
    field.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);

    pivot.RefreshData();
    pivot.CalculateData();
    Assert.AreEqual("420", book.Worksheets[0].Cells["B18"].StringValue);
    book.Save(Constants.destPath + "ValueGreaterThan.xlsx");
    book.Save(Constants.destPath + "ValueGreaterThan.pdf");
}
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


