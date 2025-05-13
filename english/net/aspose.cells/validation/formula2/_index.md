---
title: Validation.Formula2
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the value or expression associated with the data validation
type: docs
url: /net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Represents the value or expression associated with the data validation.

```csharp
public string Formula2 { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=Sheet2!B3",dv.Formula2);
public void Validation_Property_Formula2()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsb");

    Cell cell = wb.Worksheets[0].Cells["B7"];
    Validation dv = cell.GetValidation();
   Assert.AreEqual("1960-1-1",dv.Formula1);
    Assert.AreEqual("=Sheet2!B3",dv.Formula2);
    wb.Save(Constants.destPath + "example.xlsb");
}
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


