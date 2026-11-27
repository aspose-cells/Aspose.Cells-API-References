---
title: "PageSetup.FitToPagesTall"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar antalet sidor i höjd som kalkylbladet skalas till när det skrivs ut. Standardvärdet är 1"
type: docs
url: /sv/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Representerar antalet sidor i höjd som arbetsbladet skalas till när det skrivs ut. Standardvärdet är 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Anmärkningar

Du måste sätta FitToPagesWide till noll om du vill få alla rader att passa på en sida.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att få bladet att sträcka sig över flera sidor
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // Hämta PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in utskriftsområde
            pageSetup.PrintArea = "A1:J100";
            
            // Ställ in FitToPagesTall-egenskapen för att få alla rader att passa på en sida
            pageSetup.FitToPagesTall = 1;
            
            // Ställ in FitToPagesWide-egenskapen för att få alla kolumner att passa på en sida
            pageSetup.FitToPagesWide = 1;
            
            // Ställ in pappersstorlek
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Skriv ut rutnät
            pageSetup.PrintGridlines = true;

            // Skapa renderingsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Skapa bladrenderare
            SheetRender render = new SheetRender(worksheet, options);
            
            // Skriv ut sidskalan
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


