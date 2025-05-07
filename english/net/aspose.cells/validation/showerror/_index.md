---
title: Validation.ShowError
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether the data validation error message will be displayed whenever the user enters invalid data
type: docs
url: /net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

```csharp
public bool ShowError { get; set; }
```

### Examples

```csharp
// Called: validation.ShowError = true;
public static void Property_ShowError()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Define a cell area for validation
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Add a validation to the worksheet
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Set validation properties
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Save the workbook
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


