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
// Called: worksheet.HorizontalPageBreaks.Add("G5");
public static void Worksheet_Property_HorizontalPageBreaks()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a horizontal page break at row 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Add a horizontal page break at row 10, starting from column 1 to column 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Add a horizontal page break at row 15, starting from column 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Add a horizontal page break at cell "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Remove the first horizontal page break
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Save the workbook
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
            return;
        }
```

### See Also

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


