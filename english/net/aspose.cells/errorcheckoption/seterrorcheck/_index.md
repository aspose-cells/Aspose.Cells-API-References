---
title: ErrorCheckOption.SetErrorCheck
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Sets whether given error type will be checked
type: docs
url: /net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Sets whether given error type will be checked.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | error type can be checked. |
| isCheck | Boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |

### Examples

```csharp
// Called: opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
public static void Method_Boolean_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the ErrorCheckOptionCollection from the worksheet
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Add a new ErrorCheckOption to the collection
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Set error check options
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Define a cell area and add it to the ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea(&quot;A1&quot;, &quot;B10&quot;);
            opt.AddRange(ca);

            // Save the workbook
            workbook.Save(&quot;ErrorCheckOptionExample.xlsx&quot;);
            workbook.Save(&quot;ErrorCheckOptionExample.pdf&quot;);
        }
```

### See Also

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


