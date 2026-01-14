---
title: ImageOrPrintOptions.EmfType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Create ImageOrPrintOptions instance
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Set image type to EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Create SheetRender with the options
                SheetRender renderer = new SheetRender(worksheet, options);

                // Save to EMF format
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Display the EmfType property value
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Save the EMF file
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


