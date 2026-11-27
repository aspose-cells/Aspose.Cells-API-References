---
title: "ImageOrPrintOptions.DrawObjectEventHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Skapa en anpassad DrawObject‑händelsehanterare
            var drawHandler = new CustomDrawObjectEventHandler();

            // Ställ in bildalternativ med händelsehanteraren
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DrawObjectEventHandler = drawHandler;

            // Rendera kalkylbladet för att utlösa händelserna
            SheetRender render = new SheetRender(worksheet, options);
            for (int pageIndex = 0; pageIndex < render.PageCount; pageIndex++)
            {
                using (MemoryStream stream = new MemoryStream())
                {
                    render.ToImage(pageIndex, stream);
                }
            }
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Exempel: Skriv ut information om det ritade objektet
            Console.WriteLine($"Drawing {drawObject.Type} at ({x},{y}) with size {width}x{height}");
        }
    }
}
```

### Se även

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


