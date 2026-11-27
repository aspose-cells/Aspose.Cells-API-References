---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. När tecken i Excel är Unicode och inte har ställts in med korrekt teckensnitt i cellstilen kan de visas som block i pdfimage. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken först."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Anmärkningar

Standard är true.

### Exempel

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // Ställ in standardteckensnittet för arbetsboken
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Aktivera kontroll av arbetsbokens standardteckensnitt
            options.CheckWorkbookDefaultFont = true;

            // Rendera kalkylbladet till bild
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Spara bilden till fil
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


