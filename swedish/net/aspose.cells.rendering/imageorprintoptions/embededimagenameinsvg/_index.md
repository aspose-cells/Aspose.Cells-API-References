---
title: "ImageOrPrintOptions.EmbededImageNameInSvg"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Ange filnamnet för den inbäddade bilden i svg. Detta bör vara en fullständig sökväg med katalog, t.ex. cxpsEmbedded"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/
---
## ImageOrPrintOptions.EmbededImageNameInSvg property

Ange filnamnet för den inbäddade bilden i SVG. Detta bör vara en fullständig sökväg med katalog, t.ex. "c:\\xpsEmbedded"

```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Ta istället bort denna egenskap eftersom bilder nu alltid bäddas in i Svg med base64‑format. Denna egenskap kommer att tas bort 12 månader efter april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Generera en enkel bild i minnet och lägg till i kalkylbladet
            byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));

            // Skapa renderingsalternativ för bild med SVG-format
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Svg
            };

            // Visa aktuell inbäddad bildsökväg
            Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);

            // Konfigurera ny inbäddad bildkatalog
            string imageDir = "svg_embedded_images/";
            options.EmbededImageNameInSvg = imageDir;
            Directory.CreateDirectory(imageDir);

            // Rendera kalkylblad till SVG med konfigurerade alternativ
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "worksheet_output.svg");

            Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


