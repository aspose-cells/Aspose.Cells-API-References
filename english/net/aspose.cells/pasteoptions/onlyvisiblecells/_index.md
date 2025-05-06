---
title: PasteOptions.OnlyVisibleCells
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. True means only copying visible cells
type: docs
url: /net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True means only copying visible cells.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Examples

```csharp
// Called: OnlyVisibleCells = false,
public static void Property_OnlyVisibleCells()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the first worksheet
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(123);

            // Create another worksheet
            Worksheet sheet2 = workbook.Worksheets.Add(&quot;Sheet2&quot;);

            // Define the source range
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange(&quot;A1:A3&quot;);

            // Define the destination range
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange(&quot;B1:B3&quot;);

            // Create PasteOptions object
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Copy the range with the specified paste options
            destRange.Copy(sourceRange, pasteOptions);

            // Save the workbook
            workbook.Save(&quot;PasteOptionsExample.xlsx&quot;);
        }
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


