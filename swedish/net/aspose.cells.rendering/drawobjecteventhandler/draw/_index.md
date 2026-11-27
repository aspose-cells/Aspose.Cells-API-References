---
title: "DrawObjectEventHandler.Draw"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObjectEventHandler‑metod. Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering"
type: docs
url: /sv/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject kommer att initieras och returneras vid rendering |
| x | Single | Vänster om DrawObject |
| y | Single | Övre kant av DrawObject |
| bredd | Single | Bredd på DrawObject |
| höjd | Single | Höjd på DrawObject |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawObjectEventHandlerMethodDrawWithDrawObjectSingleSingleSingleSiDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells Drawing Demo";

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                sheetRender.ToImage(0, "DrawDemoOutput.png");
                Console.WriteLine("Draw method executed during rendering. Output saved to DrawDemoOutput.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }

        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Denna implementation kommer att anropas under rendering för varje DrawObject
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### Se även

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


