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
// Called: object[] itemArray = (object[])validationForA1.Value1;
[Test]
        public void Property_Value1()
        {
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            Workbook wkbook = new Workbook(Constants.sourcePath + "CELLSNET44169.xlsx", options);

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

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


