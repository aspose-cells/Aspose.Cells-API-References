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
// Called: validation.ErrorTitle = &amp;quot;Invalid Input&amp;quot;;
public static void Property_ErrorTitle()
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
            validation.Formula1 = &quot;3&quot;;
            validation.Formula2 = &quot;1234&quot;;

            // Set additional properties for the validation
            validation.InputMessage = &quot;Please enter a whole number between 3 and 1234.&quot;;
            validation.InputTitle = &quot;Whole Number Validation&quot;;
            validation.ErrorMessage = &quot;The value must be a whole number between 3 and 1234.&quot;;
            validation.ErrorTitle = &quot;Invalid Input&quot;;
            validation.ShowInput = true;
            validation.ShowError = true;

            // Save the workbook
            workbook.Save(&quot;ValidationTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


