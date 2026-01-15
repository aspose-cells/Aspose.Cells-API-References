---
title: Font.Name
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the name of the Font
type: docs
url: /net/aspose.cells/font/name/
---
## Font.Name property

Gets or sets the name of the [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Remarks

If this property is used to set the name of the font, the [`SchemeType`](../schemetype/) will be updated to None

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the default worksheet and cells
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Create and modify a style with font properties
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Demonstrate Name property usage
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Apply the style to a cell
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Save the workbook
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


