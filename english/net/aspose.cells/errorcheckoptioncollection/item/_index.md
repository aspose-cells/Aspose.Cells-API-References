---
title: ErrorCheckOptionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOptionCollection property. Gets ErrorCheckOption object by the given index
type: docs
url: /net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Gets [`ErrorCheckOption`](../../errorcheckoption/) object by the given index.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Return Value

Return [`ErrorCheckOption`](../../errorcheckoption/) object

### Examples

```csharp
// Called: ErrorCheckOption opt = opts[optionIdx];
public static void ErrorCheckOptionCollection_Property_Item()
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

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


