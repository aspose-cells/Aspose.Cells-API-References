---
title: Validation.AlertStyle
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the validation alert style
type: docs
url: /net/aspose.cells/validation/alertstyle/
---
## Validation.AlertStyle property

Represents the validation alert style.

```csharp
public ValidationAlertType AlertStyle { get; set; }
```

### Examples

```csharp
// Called: validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
public static void Validation_Property_AlertStyle()
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

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


