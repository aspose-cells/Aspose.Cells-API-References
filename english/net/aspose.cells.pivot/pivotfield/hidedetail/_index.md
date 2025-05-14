---
title: PivotField.HideDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field
type: docs
url: /net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.

```csharp
public void HideDetail(bool isHiddenDetail)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | Boolean | Whether hide the detail of the pivot field. |

### Examples

```csharp
// Called: field.HideDetail(true);
public void PivotField_Method_HideDetail()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.HideDetail(true);

    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("Japan", cells["A19"].StringValue);

    book.Save(Constants.destPath + "TestHideDetail.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


