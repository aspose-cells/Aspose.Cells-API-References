---
title: Validation.ErrorTitle
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the title of the datavalidation error dialog box
type: docs
url: /net/aspose.cells/validation/errortitle/
---
## Validation.ErrorTitle property

Represents the title of the data-validation error dialog box.

```csharp
public string ErrorTitle { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("altet tiltle", dv.ErrorTitle);
[Test]
        public void Property_ErrorTitle()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41325_1.ods");

            Assert.AreEqual(11,workbook.Worksheets[0].Validations.Count);
            Validation dv = workbook.Worksheets[0].Cells["A1"].GetValidation();

            Assert.AreEqual("altet tiltle",dv.ErrorTitle);
           Assert.AreEqual(Aspose.Cells.ValidationType.WholeNumber ,dv.Type);
            workbook.Save(Constants.destPath + "CELLSJAVA41325_1.ods");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA41325_1.ods");

            Assert.AreEqual(11, workbook.Worksheets[0].Validations.Count);
             dv = workbook.Worksheets[0].Cells["A1"].GetValidation();

            Assert.AreEqual("altet tiltle", dv.ErrorTitle);
            Assert.AreEqual(Aspose.Cells.ValidationType.WholeNumber, dv.Type);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


