---
title: ErrorCheckOption.AddRange
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Adds one influenced range by this setting
type: docs
url: /net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Adds one influenced range by this setting.

```csharp
public int AddRange(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the range to be added. |

### Return Value

the index of the added range in the range list of this setting.

### Examples

```csharp
// Called: opt.AddRange(ca);
public static void Method_CellArea_()
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
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Save the workbook
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


