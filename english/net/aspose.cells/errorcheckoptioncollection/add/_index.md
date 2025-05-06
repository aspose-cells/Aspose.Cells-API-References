---
title: ErrorCheckOptionCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOptionCollection method. Add an error check option
type: docs
url: /net/aspose.cells/errorcheckoptioncollection/add/
---
## ErrorCheckOptionCollection.Add method

Add an error check option.

```csharp
public int Add()
```

### Examples

```csharp
// Called: int optionIndex = errorCheckOptions.Add();
public static void Method_Add()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Add a new ErrorCheckOption
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Set various error check types to false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Define a cell area for the error check option
            CellArea cellArea = CellArea.CreateCellArea(&quot;A1&quot;, &quot;B10&quot;);
            errorCheckOption.AddRange(cellArea);

            // Save the workbook
            workbook.Save(&quot;ErrorCheckTypeExample.xlsx&quot;);
            workbook.Save(&quot;ErrorCheckTypeExample.pdf&quot;);
        }
```

### See Also

* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


