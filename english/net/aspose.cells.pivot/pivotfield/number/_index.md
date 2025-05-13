---
title: PivotField.Number
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the builtin display format of numbers and dates
type: docs
url: /net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Represents the built-in display format of numbers and dates.

```csharp
public int Number { get; set; }
```

### Examples

```csharp
// Called: field.Number = 16;
public void PivotField_Property_Number()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.ColumnFields[0];
    field.Number = 16;
    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("8-Jan", cells["C17"].StringValue);
    book.Save(Constants.destPath + "TestNumber.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


