---
title: Outline.SummaryColumnRight
second_title: Aspose.Cells for .NET API Reference
description: Outline property. Indicates if the summary column will be positioned to the right of the detail columns in the outline
type: docs
url: /net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Indicates if the summary column will be positioned to the right of the detail columns in the outline.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Examples

```csharp
// Called: outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
public static void Property_SummaryColumnRight()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the outline of the worksheet
            Outline outline = worksheet.Outline;
            
            // Set the properties of the outline
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Save the workbook
            workbook.Save("OutlineExample.xlsx");

            return;
        }
```

### See Also

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


