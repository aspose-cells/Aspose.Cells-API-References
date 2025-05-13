---
title: PivotField.IsHiddenItemDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets whether hidding the detail of the specific PivotItem
type: docs
url: /net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Gets whether hidding the detail of the specific PivotItem..

```csharp
public bool IsHiddenItemDetail(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the pivotItem in the pivotField. |

### Return Value

whether the specific PivotItem is hidden detail

### Examples

```csharp
// Called: Assert.AreEqual(true, field.IsHiddenItemDetail(1));
public void PivotField_Method_IsHiddenItemDetail()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.HideItemDetail(1, true);

    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual(true, field.IsHiddenItemDetail(1));
    Assert.AreEqual("Japan", cells["A23"].StringValue);

    book.Save(Constants.destPath + "TestHideItemDetail.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


