---
title: PivotField.Function
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the function used to summarize the PivotTable data field
type: docs
url: /net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Represents the function used to summarize the PivotTable data field.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Examples

```csharp
// Called: field.Function = ConsolidationFunction.Max;
public void PivotField_Property_Function()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];
    Cells cells = sheet.Cells;
    PivotField field = pivot.DataFields[0];
    field.Function = ConsolidationFunction.Max;
    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("120", cells["O33"].StringValue);
    book.Save(Constants.destPath + "TestFunction.xlsx");
}
```

### See Also

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


