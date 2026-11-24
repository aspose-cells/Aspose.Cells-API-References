---
title: "DrawObjectEventHandler.Draw"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObjectEventHandler-Methode. Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten"
type: docs
url: /de/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Implementiert dieses Interface, um beim Rendern DrawObject und Bound zu erhalten.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject wird beim Rendern initialisiert und zurückgegeben |
| x | Einzeln | Links von DrawObject |
| y | Einzeln | Oben von DrawObject |
| Breite | Einzeln | Breite von DrawObject |
| Höhe | Einzeln | Höhe von DrawObject |

### Beispiele

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
                // Diese Implementierung wird während des Renderns für jedes DrawObject aufgerufen
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### Siehe auch

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


