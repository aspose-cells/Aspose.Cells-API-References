---
title: "SheetRender.ToTiff"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetRender‑metod. Rendera hela kalkylbladet som en Tiff‑bild till en ström"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Rendera hela kalkylbladet som Tiff Image till en ström.

```csharp
public void ToTiff(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | strömmen för den utgående bilden |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempelinnehåll för att demonstrera rendering
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Konfigurera bildalternativ för rendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Skapa bladrenderare med konfigurerade alternativ
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // Skapa utdataflöde för TIFF-bild
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Rendera kalkylblad till TIFF med hjälp av flöde
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Rendera hela kalkylbladet som Tiff Image till en fil.

```csharp
public void ToTiff(string filename)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | String | filnamnet för den utgående bilden |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // Läs in käll-Excel-filen
            Workbook workbook = new Workbook("Book1.xlsx");

            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // Skapa sheet render för det första kalkylbladet
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Spara alla sidor i bladet som en flersidig TIFF-fil
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


