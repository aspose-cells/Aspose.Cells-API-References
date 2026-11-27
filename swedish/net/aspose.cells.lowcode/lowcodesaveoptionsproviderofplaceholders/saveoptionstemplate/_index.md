---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders egenskap. Mallen för att skapa en instans av sparalternativ i GetSaveOptions"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate property

Mallen för att skapa en instans av sparalternativ i [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Anmärkningar

Om mallen har angetts kommer den skapade instansen att kopiera alla inställningar från den och uppdatera utdatafilen i enlighet med detta.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            
            // Initiera leverantören med sökvägsmall som innehåller platshållare
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/Sheet_{sheet}_Part_{part}.pdf");
            
            // Visa det initiala malltillståndet
            Console.WriteLine($"Initial SaveOptionsTemplate: {(provider.SaveOptionsTemplate == null ? "Not set" : "Configured")}");
            
            // Skapa och konfigurera ny mall för sparalternativ
            provider.SaveOptionsTemplate = new LowCodePdfSaveOptions
            {
                PdfOptions = new PdfSaveOptions  // Fixed property name from PdfSaveOptions to PdfOptions
                {
                    Compliance = PdfCompliance.PdfA1a,
                    ExportDocumentStructure = true
                }
            };

            // Konfigurera delningsparametrar
            provider.BuildPathWithSheetAlways = true;
            provider.SplitPartPrefix = "Split_";
            
            // Visa konfigurerade PDF-alternativ
            var pdfOptions = (LowCodePdfSaveOptions)provider.SaveOptionsTemplate;
            Console.WriteLine($"Configured PDF Compliance: {pdfOptions.PdfOptions.Compliance}");  // Fixed property access
            Console.WriteLine($"Document Structure Export: {pdfOptions.PdfOptions.ExportDocumentStructure}");  // Fixed property access

            // Lägg till sidbrytning för att skapa delade delar
            worksheet.HorizontalPageBreaks.Add(0);
            
            // Spara med leverantörens konfiguration (faktisk delning/sparning skulle ske här)
            Console.WriteLine("Workbook prepared with SaveOptionsTemplate configuration");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


