---
title: "SheetRender.SheetRender"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetRender‑konstruktor. konstruktionen av SheetRender kräver ett kalkylblad och ImageOrPrintOptions som parametrar"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

Konstruktionen av SheetRender, behöver kalkylblad och ImageOrPrintOptions som parametrar

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| worksheet | Arbetsblad | Ange vilket kalkylblad som ska renderas. |
| alternativ | ImageOrPrintOptions | ImageOrPrintOptions innehåller vissa egenskaper för utdatabild |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa bild-/utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Skapa SheetRender med Worksheet och ImageOrPrintOptions
            SheetRender render = new SheetRender(worksheet, options);

            // Utdata sidantal
            Console.WriteLine("Page count: " + render.PageCount);

            // Spara den renderade bilden
            render.ToImage(0, "output.png");
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


