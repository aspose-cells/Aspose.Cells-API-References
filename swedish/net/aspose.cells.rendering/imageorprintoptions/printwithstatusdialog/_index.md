---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Om PrintWithStatusDialog är true visas en dialog som visar aktuell utskriftsstatus. Annars visas ingen sådan dialog."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

Om PrintWithStatusDialog = true visas en dialog som visar aktuell utskriftsstatus. Annars visas ingen sådan dialog.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Initiera en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Ställ in bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // Skapa bladrendering
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // Skriv ut till PDF
            sheetRender.ToImage(0, "output.png");

            // Vänta på att filen skapas (förenklad väntelogik)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


