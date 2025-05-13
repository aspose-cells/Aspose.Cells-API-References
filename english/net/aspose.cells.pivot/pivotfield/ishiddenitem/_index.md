---
title: PivotField.IsHiddenItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets whether the specific PivotItem is hidden
type: docs
url: /net/aspose.cells.pivot/pivotfield/ishiddenitem/
---
## PivotField.IsHiddenItem method

Gets whether the specific PivotItem is hidden.

```csharp
public bool IsHiddenItem(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the pivotItem in the pivotField. |

### Return Value

whether the specific PivotItem is hidden

### Examples

```csharp
// Called: Assert.AreEqual(true, field.IsHiddenItem(1));
public void PivotField_Method_IsHiddenItem()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.HideItem(1, true);
    pivot.RefreshData();
    pivot.CalculateData();
    Assert.AreEqual(true, field.IsHiddenItem(1));

    Assert.AreEqual("USA", cells["A23"].StringValue);

    book.Save(Constants.destPath + "TestHideItem.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


