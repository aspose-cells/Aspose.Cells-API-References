---
title: "ImageOrPrintOptions.EmfType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger en EmfType som specificerar formatet för Metafile. Standardvärdet är EmfPlusDual"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Hämtar eller anger en EmfType som specificerar formatet för Metafilen. Standardvärdet är EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Skapa en ImageOrPrintOptions-instans
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Ställ in bildtyp till EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Skapa SheetRender med alternativen
                SheetRender renderer = new SheetRender(worksheet, options);

                // Spara i EMF-format
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Visa värdet för egenskapen EmfType
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Spara EMF-filen
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

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


