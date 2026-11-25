---
title: "DrawObjectEventHandler.Draw"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DrawObjectEventHandler. Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject verrà inizializzato e restituito durante il rendering |
| x | Single | Sinistra di DrawObject |
| y | Single | Alto di DrawObject |
| larghezza | Single | Larghezza di DrawObject |
| altezza | Single | Altezza di DrawObject |

### Esempi

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
                // Questa implementazione verrà chiamata durante il rendering per ogni DrawObject
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### Vedi anche

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


