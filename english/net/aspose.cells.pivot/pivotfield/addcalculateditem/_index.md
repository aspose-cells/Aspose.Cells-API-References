---
title: PivotField.AddCalculatedItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Add a calculated formula item to the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

Add a calculated formula item to the pivot field.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The item's name. |
| formula | String | The formula of pivot item. |

### Remarks

Only supports to add calculated item to Row/Column field.

### Examples

```csharp
// Called: field.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
public void PivotField_Method_AddCalculatedItem()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[1];
    field.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
    pivot.RefreshData();
    pivot.CalculateData();

    //Assert.AreEqual("grape_kiwi_total", cells["B22"].StringValue);
    //Assert.AreEqual("120", cells["O22"].StringValue);
    book.Save(Constants.destPath + "TestAddCalculatedItem.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


