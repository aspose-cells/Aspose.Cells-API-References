---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger om utdataelementen ska optimeras"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Anger om utdataelementen ska optimeras.

```csharp
public bool IsOptimized { get; set; }
```

### Anmärkningar

Standardvärdet är false. För närvarande, när denna egenskap är satt till true, kommer följande optimeringar att utföras: 1. optimera kantlinjerna. 2. optimera filstorleken vid rendering till Svg-bild.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // Ställ in alternativ för bildrendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Demonstrera IsOptimized-egenskapen
            options.IsOptimized = true; // Enable optimization
            
            // Rendera bladet till bild
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


