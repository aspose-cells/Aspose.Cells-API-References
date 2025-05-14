---
title: PivotField.InsertBlankRow
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether inserting blank line after each item
type: docs
url: /net/aspose.cells.pivot/pivotfield/insertblankrow/
---
## PivotField.InsertBlankRow property

Indicates whether inserting blank line after each item.

```csharp
public bool InsertBlankRow { get; set; }
```

### Examples

```csharp
// Called: field.InsertBlankRow = true;
public void PivotField_Property_InsertBlankRow()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];
    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.InsertBlankRow = true;
    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("", cells["A23"].StringValue);
    Assert.AreEqual("", cells["A29"].StringValue);
    Assert.AreEqual("", cells["A35"].StringValue);
    book.Save(Constants.destPath + "TestInsertBlankRow.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


