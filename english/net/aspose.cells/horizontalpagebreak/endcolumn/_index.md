---
title: HorizontalPageBreak.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the end column index of this horizontal page break
type: docs
url: /net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Gets the end column index of this horizontal page break.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($&amp;quot;End Column: {hPageBreak.EndColumn}&amp;quot;);
public static void Property_EndColumn()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a page break at cell Y30
            int index = worksheet.HorizontalPageBreaks.Add(&quot;Y30&quot;);
            
            // Get the newly added horizontal page break
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Display the properties of the horizontal page break
            Console.WriteLine(&quot;Horizontal Page Break Details:&quot;);
            Console.WriteLine($&quot;Row: {hPageBreak.Row}&quot;);
            Console.WriteLine($&quot;Start Column: {hPageBreak.StartColumn}&quot;);
            Console.WriteLine($&quot;End Column: {hPageBreak.EndColumn}&quot;);
            
            // Save the workbook
            workbook.Save(&quot;HorizontalPageBreakExample.xlsx&quot;);
            workbook.Save(&quot;HorizontalPageBreakExample.pdf&quot;);
        }
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


