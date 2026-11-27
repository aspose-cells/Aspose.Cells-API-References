---
title: "PdfSaveOptions.ImageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions‑egenskap. Representerar bildtypen när diagram och form konverteras"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Representerar bildtypen när diagram och form konverteras.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Istället renderas Chart och Shape alltid som vektorelement (t.ex. point, line) för renderingskvalitet. Denna egenskap kommer att tas bort 12 månader senare sedan juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelarbetsblad med några data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // Skapa PDF-sparalternativ
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Visa standardvärdet för ImageType
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Ange ett annat ImageType‑värde
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Spara arbetsboken som PDF med den angivna ImageType
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


