---
title: "Klass LowCodeImageSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeImageSaveOptions-klass. Alternativ för att spara bild på ett lågkodssätt"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Alternativ för att spara bild på ett lågt kodsätt.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | Alternativen för att rendera bilder. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Hämtar och anger filen (med sökväg om behövs) för att spara den genererade datan. När denna egenskap sätts till ett värde annat än null eller tom sträng, kommer [`OutputStream`](../lowcodesaveoptions/outputstream/) att ignoreras. (Arv från [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Hämtar och anger strömmen för att skriva den genererade datan till. När den här egenskapen sätts till ett värde annat än null, kommer [`OutputFile`](../lowcodesaveoptions/outputfile/) att ignoreras. (Ärvd från [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Hämtar eller anger sparaformatet. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Leverantör av sparaalternativ för att spara genererade bilder. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata i kalkylbladet
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // Skapa en instans av LowCodeImageSaveOptions
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // Ställ in grundläggande egenskaper
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // Visa aktuella inställningar
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // Ändra några bildalternativ
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // Skapa en enkel leverantör av sparaalternativ
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // Spara kalkylbladet som en bild
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


