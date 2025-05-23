---
title: Worksheet.VerticalPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the VerticalPageBreakCollection collection
type: docs
url: /net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Gets the [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/) collection.

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Examples

```csharp
// Called: VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
public static void Worksheet_Property_VerticalPageBreaks()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the VerticalPageBreakCollection of the worksheet
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Add vertical page breaks
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add("G5"); // At cell G5

            // Remove a vertical page break at index 1
            verticalPageBreaks.RemoveAt(1);

            // Access and print details of the vertical page breaks
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Save the workbook
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


