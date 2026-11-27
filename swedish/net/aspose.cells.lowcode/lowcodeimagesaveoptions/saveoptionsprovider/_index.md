---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeImageSaveOptions‑egenskap. Leverantör av spara‑alternativ för att spara genererade bilder"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Leverantör av sparaalternativ för att spara genererade bilder.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Anmärkningar

Utdata([`OutputFile`](../../lowcodesaveoptions/outputfile/) eller [`OutputStream`](../../lowcodesaveoptions/outputstream/)) som anges av detta objekt kommer inte att ha någon effekt när denna egenskap är specificerad. Istället kommer utdata för varje genererad bild att anges av leverantören.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // Skapa en LowCodeImageSaveOptions‑instans
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Skapa en anpassad SaveOptionsProvider
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Visa aktuell SaveOptionsProvider
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Demonstrera effekten genom att spara med olika alternativ
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Byt till null‑leverantör
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Returnera anpassade spara‑alternativ för varje del
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Utför eventuell städning efter sparning
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### Se även

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


