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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and get the first worksheet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Choose a cell to store the embedded image
                Cell cell = worksheet.Cells["B2"];

                // A 1x1 pixel transparent PNG (Base64 encoded)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Convert the Base64 string to a byte array
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Set the embedded image into the cell
                cell.EmbeddedImage = imageBytes;

                // Retrieve the embedded image back from the cell
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Write the retrieved image to a file to verify it was stored correctly
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Save the workbook (the embedded image is stored inside the .xlsx)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


