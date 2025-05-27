---
title: Cell.EmbeddedImage
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets and sets the embeddedn image in the cell
type: docs
url: /net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Gets and sets the embeddedn image in the cell.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using System.IO;

namespace AsposeCellsExamples
{
    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Load an image file
            byte[] imageData = File.ReadAllBytes("example.png");

            // Add the image to cell A1 using MemoryStream
            using (MemoryStream stream = new MemoryStream(imageData))
            {
                worksheet.Pictures.Add(0, 0, stream);
            }
            
            // Access the embedded image from cell A1
            Aspose.Cells.Drawing.Picture embeddedImage = worksheet.Pictures[0];
            
            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


