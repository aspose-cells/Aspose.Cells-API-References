---
title: "Class DrawObjectEventHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.DrawObjectEventHandler klass. Gränssnitt för att hämta DrawObject och Bound vid rendering"
type: docs
url: /sv/net/aspose.cells.rendering/drawobjecteventhandler/
---
## DrawObjectEventHandler class

Gränssnitt för att hämta DrawObject och Bound vid rendering.

```csharp
public abstract class DrawObjectEventHandler
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(12345);
            worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter

            // Skapa PDF‑sparalternativ med anpassad render‑hanterare
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();

            // Spara arbetsbok till PDF med anpassning av rendering
            workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Demonstrera hantering av olika renderingsobjekttyper
            switch (drawObject.Type)
            {
                case DrawObjectEnum.Cell:
                    Console.WriteLine($"Rendering cell at ({x}, {y})");
                    break;
                    
                case DrawObjectEnum.Image:
                    Console.WriteLine($"Rendering image at ({x}, {y})");
                    break;
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


