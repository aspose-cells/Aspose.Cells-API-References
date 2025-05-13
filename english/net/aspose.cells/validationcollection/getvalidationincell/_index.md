---
title: ValidationCollection.GetValidationInCell
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection method. Gets the validation applied to given cell
type: docs
url: /net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Gets the validation applied to given cell.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

Returns a [`Validation`](../../validation/) object or null if there is no validation for given cell

### Examples

```csharp
// Called: var validationForA1 = wksheet.Validations.GetValidationInCell(0, 0);
public void ValidationCollection_Method_GetValidationInCell()
{
    LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
    Workbook wkbook = new Workbook(Constants.sourcePath + "example.xlsx", options);

    Worksheet wksheet = wkbook.Worksheets[0];

    var validationForA1 = wksheet.Validations.GetValidationInCell(0, 0);
    if (validationForA1.Type == ValidationType.List)
    {
        StringBuilder sbuf = new StringBuilder();
        object[] itemArray = (object[])validationForA1.Value1;
        Assert.AreEqual((string)itemArray[0], "(none)"); 
    }
}
```

### See Also

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


