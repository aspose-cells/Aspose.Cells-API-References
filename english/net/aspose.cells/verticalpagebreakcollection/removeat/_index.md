---
title: VerticalPageBreakCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreakCollection method. Removes the VPageBreak element at a specified name
type: docs
url: /net/aspose.cells/verticalpagebreakcollection/removeat/
---
## VerticalPageBreakCollection.RemoveAt method

Removes the VPageBreak element at a specified name.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Element index, zero based. |

### Examples

```csharp
// Called: verticalPageBreaks.RemoveAt(1);
public static void Method_Int32_()
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
            verticalPageBreaks.Add(&quot;G5&quot;); // At cell G5

            // Remove a vertical page break at index 1
            verticalPageBreaks.RemoveAt(1);

            // Access and print details of the vertical page breaks
            for (int i = 0; i &lt; verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($&quot;Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;VerticalPageBreakCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


