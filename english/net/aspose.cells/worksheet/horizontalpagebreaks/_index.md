---
title: Worksheet.HorizontalPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the HorizontalPageBreakCollection collection
type: docs
url: /net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Gets the [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/) collection.

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Examples

```csharp
// Called: int index = worksheet.HorizontalPageBreaks.Add("Y30");
public static void Property_HorizontalPageBreaks()
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

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


