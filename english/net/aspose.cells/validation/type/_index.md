---
title: Validation.Type
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the data validation type
type: docs
url: /net/aspose.cells/validation/type/
---
## Validation.Type property

Represents the data validation type.

```csharp
public ValidationType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(Aspose.Cells.ValidationType.WholeNumber ,dv.Type);
public void Validation_Property_Type()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");

    Assert.AreEqual(11,workbook.Worksheets[0].Validations.Count);
    Validation dv = workbook.Worksheets[0].Cells["A1"].GetValidation();

    Assert.AreEqual("altet tiltle",dv.ErrorTitle);
   Assert.AreEqual(Aspose.Cells.ValidationType.WholeNumber ,dv.Type);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");

    Assert.AreEqual(11, workbook.Worksheets[0].Validations.Count);
     dv = workbook.Worksheets[0].Cells["A1"].GetValidation();

    Assert.AreEqual("altet tiltle", dv.ErrorTitle);
    Assert.AreEqual(Aspose.Cells.ValidationType.WholeNumber, dv.Type);
}
```

### See Also

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


