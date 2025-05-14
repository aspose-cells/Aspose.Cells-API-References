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
// Called: validation.ErrorTitle = "Invalid Input";
public static void Validation_Property_ErrorTitle()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a validation to the worksheet
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Set validation type to WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Set additional properties for the validation
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Save the workbook
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


