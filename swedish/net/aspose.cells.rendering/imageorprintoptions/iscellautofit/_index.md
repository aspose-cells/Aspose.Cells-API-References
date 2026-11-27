---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

Anger om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. Standardvärdet är falskt.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Istället används inte denna egenskap, vänligen ta bort denna egenskap.. Denna egenskap kommer att tas bort 12 månader senare sedan augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeltext som överskrider standardkolumnbredden
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // Skapa alternativ för bildrendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Demonstrera IsCellAutoFit falskt (standard)
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // Ändra IsCellAutoFit till true
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // Konfigurera bildformat
            options.ImageType = ImageType.Png;

            // Rendera kalkylblad till bild med angivna alternativ
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


