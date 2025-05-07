---
title: Validation.IgnoreBlank
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether blank values are permitted by the range data validation
type: docs
url: /net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Indicates whether blank values are permitted by the range data validation.

```csharp
public bool IgnoreBlank { get; set; }
```

### Examples

```csharp
// Called: validation.IgnoreBlank = true;
[Test]
        public void Property_IgnoreBlank()
        {
            Workbook workbook = new Workbook();

            ValidationCollection validations = workbook.Worksheets[0].Validations;
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 1;
            area.StartColumn = 0;
            area.EndColumn = 1;
            Validation validation = validations[validations.Add(area)];

            //Setting the validation type to whole number

            validation.Type = Aspose.Cells.ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "2";
            validation.Formula2 = "20";
            validation.ErrorMessage = "Error....";
            validation.IgnoreBlank = true;
            //Applying the validation to a range of cells from A1 to B2 using the
            //CellArea structure
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells.InsertRows(0, 2);
            Assert.AreEqual(validation.Formula1,"=2"); //=20...wrong
            Assert.AreEqual(validation.Formula2,"=20"); //20...right
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


