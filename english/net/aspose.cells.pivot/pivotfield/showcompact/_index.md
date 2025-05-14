---
title: PivotField.ShowCompact
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether display labels from the next field in the same column on the Pivot Table view
type: docs
url: /net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Indicates whether display labels from the next field in the same column on the Pivot Table view

```csharp
public bool ShowCompact { get; set; }
```

### Examples

```csharp
// Called: field.ShowCompact = true;
public void PivotField_Property_ShowCompact()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.ShowInOutlineForm = true;
    field.ShowCompact = true;
    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("grape", cells["A19"].StringValue);
    book.Save(Constants.destPath + "TestShowCompact.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


