---
title: PivotField.IsAutoSort
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is automatically sorted
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Indicates whether the specified PivotTable field is automatically sorted.

```csharp
public bool IsAutoSort { get; set; }
```

### Examples

```csharp
// Called: field.IsAutoSort = true;
public void PivotField_Property_IsAutoSort()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];
    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[1];
    field.IsAutoSort = true;
    field.AutoSortField = 0;
    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("blueberry", cells["B30"].StringValue);
    book.Save(Constants.destPath + "TestAutoSortField.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


