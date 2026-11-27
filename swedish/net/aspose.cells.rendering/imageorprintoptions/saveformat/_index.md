---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger filformatstyp för utdata. Stöder Tiff/XPS"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Hämtar eller anger filformatstyp för utdata. Stöder Tiff/XPS

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället för Tiff/Svg [`ImageType`](../imagetype/); för Xps, använd [`Save`](../../../aspose.cells/workbook/save/) med [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och fyll i exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // Skapa en ImageOrPrintOptions-instans
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Visa initiala SaveFormat‑värdet
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Ställ in SaveFormat till TIFF och rendera kalkylbladet
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // Ändra SaveFormat till XPS och rendera igen
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Obs: SheetRender stöder inte XPS‑format. Detta sparas istället som bildformat.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### Se även

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


