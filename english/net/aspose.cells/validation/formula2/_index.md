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
// Called: validation.Formula2 = &amp;quot;1234&amp;quot;;
public static void Property_Formula2()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Define a cell area for the validation
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Access the validations collection
            ValidationCollection validations = worksheet.Validations;

            // Add a new validation to the collection
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Set validation properties
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = &quot;3&quot;;
            validation.Formula2 = &quot;1234&quot;;
            validation.InputMessage = &quot;Please enter a whole number between 3 and 1234.&quot;;
            validation.InputTitle = &quot;Whole Number Validation&quot;;
            validation.ErrorMessage = &quot;The value must be a whole number between 3 and 1234.&quot;;
            validation.ErrorTitle = &quot;Invalid Input&quot;;
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // Save the workbook
            workbook.Save(&quot;ValidationExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


