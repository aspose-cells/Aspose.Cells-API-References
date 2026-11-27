---
title: "ImageOrPrintOptions.OnlyArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Om denna egenskap är sann kommer ett område att skrivas ut och ingen skalning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

Om denna egenskap är sann, kommer ett område att skrivas ut och ingen skalning kommer att tillämpas.

```csharp
public bool OnlyArea { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnlyAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Ställ in bildalternativ med OnlyArea-egenskap
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnlyArea = true; // Only render the used area

            // Rendera kalkylblad till bild
            SheetRender sr = new SheetRender(worksheet, options);
            using (MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, ms);
                Console.WriteLine("Worksheet rendered to image with OnlyArea=true");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


