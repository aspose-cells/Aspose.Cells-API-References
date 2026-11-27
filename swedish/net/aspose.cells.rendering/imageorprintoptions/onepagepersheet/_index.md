---
title: "ImageOrPrintOptions.OnePagePerSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut till endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig och de andra inställningarna för pagesetup kommer fortfarande att tillämpas."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Sample Data for OnePagePerSheet Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Row " + i);
            }

            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true; // Key property being demonstrated
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Skapa bladrendering
            SheetRender sr = new SheetRender(worksheet, options);
            
            // Spara den genererade bilden
            sr.ToImage(0, "OnePagePerSheetOutput.png");
            
            Console.WriteLine("Output saved with OnePagePerSheet=true");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


