---
title: Validation.Value1
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the first value associated with the data validation
type: docs
url: /net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Represents the first value associated with the data validation.

```csharp
public object Value1 { get; set; }
```

### Examples

```csharp
// Called: vals = val.Value1 as object[];
public void Validation_Property_Value1()
{
    Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Validation val = workbook.Worksheets[0].Cells["D12"].GetValidation();
    object[] vals = val.Value1 as object[];
    Assert.AreEqual((string)vals[0],"Bitte wählen");

     workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xls");
    val = workbook.Worksheets[6].Cells["D12"].GetValidation();
    vals = val.Value1 as object[];
    Assert.AreEqual((string)vals[0], "Bitte wählen");
}
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


