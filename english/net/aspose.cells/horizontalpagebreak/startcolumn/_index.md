---
title: HorizontalPageBreak.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the start column index of this horizontal page break
type: docs
url: /net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Gets the start column index of this horizontal page break.

```csharp
public int StartColumn { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
public static void HorizontalPageBreak_Property_StartColumn()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a page break at cell Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Get the newly added horizontal page break
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Display the properties of the horizontal page break
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Save the workbook
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


