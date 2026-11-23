---
title: "DrawObjectEventHandler.Draw"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DrawObjectEventHandler. Implémente cette interface pour obtenir DrawObject et Bound lors du rendu"
type: docs
url: /fr/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject sera initialisé et renvoyé lors du rendu |
| x | Single | Gauche de DrawObject |
| y | Single | Haut de DrawObject |
| largeur | Single | Largeur de DrawObject |
| hauteur | Single | Hauteur de DrawObject |

### Exemples

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
                // Cette implémentation sera appelée pendant le rendu pour chaque DrawObject
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### Voir aussi

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


