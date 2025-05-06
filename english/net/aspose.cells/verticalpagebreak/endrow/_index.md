---
title: VerticalPageBreak.EndRow
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreak property. Gets the end row index of the vertical page break
type: docs
url: /net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Gets the end row index of the vertical page break.

```csharp
public int EndRow { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;End Row: &amp;quot; + vpb.EndRow);
public static void Property_EndRow()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a vertical page break at column G (index 6)
            worksheet.VerticalPageBreaks.Add(&quot;G5&quot;);

            // Save the workbook
            workbook.Save(&quot;VerticalPageBreakExample.xlsx&quot;);

            // Access the added vertical page break
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Display the properties of the vertical page break
            Console.WriteLine(&quot;Start Row: &quot; + vpb.StartRow);
            Console.WriteLine(&quot;End Row: &quot; + vpb.EndRow);
            Console.WriteLine(&quot;Column: &quot; + vpb.Column);
        }
```

### See Also

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


