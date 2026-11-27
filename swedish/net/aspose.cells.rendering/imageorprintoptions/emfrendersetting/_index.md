---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Inställning för rendering av Emf-metafiler i källfilen"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Inställning för rendering av Emf‑metafiler i källfilen.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Anmärkningar

EMF-metafiler identifierade som "EMF+ Dual" kan innehålla både EMF+-poster och EMF-poster. Båda typer av poster kan användas för att rendera bilden, endast EMF+-poster, eller endast EMF-poster. När EmfPlusPrefer är inställt, kommer EMF+-poster att parsas vid rendering till bild, annars parsas endast EMF-poster. Standardvärdet är EmfOnly. För de ramverk som är beroende av .NET System.Drawing.Common ignoreras denna inställning.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med testinnehåll
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Skapa alternativ för bildrendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Visa aktuell inställning
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Rendera med standardinställningar för EMF
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // Ändra EMF-renderingsinställning och rendera igen
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### Se även

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


