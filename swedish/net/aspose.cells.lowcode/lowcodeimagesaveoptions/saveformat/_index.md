---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeImageSaveOptions‑egenskap. Hämtar eller anger spara‑formatet"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Hämtar eller anger sparaformatet.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Anmärkningar

Om [`ImageOptions`](../imageoptions/) har angetts, kommer inställning av denna egenskap också att ändra [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/)‑värdet för den.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // Initiera LowCodeImageSaveOptions med standardvärden
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // Visa initiala SaveFormat (standard är Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Konfigurera för JPEG‑utdata
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // Byt till PNG‑format och spara igen
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Rendera kalkylblad med de konfigurerade alternativen
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### Se även

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


