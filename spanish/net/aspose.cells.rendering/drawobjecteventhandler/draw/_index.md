---
title: "DrawObjectEventHandler.Draw"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DrawObjectEventHandler. Implementa esta interfaz para obtener DrawObject y Bound al renderizar"
type: docs
url: /es/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Implemente esta interfaz para obtener DrawObject y Bound al renderizar.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject será inicializado y devuelto al renderizar |
| x | Single | Izquierda de DrawObject |
| y | Single | Superior de DrawObject |
| ancho | Single | Ancho de DrawObject |
| altura | Single | Altura de DrawObject |

### Ejemplos

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
                // Esta implementación será llamada durante el renderizado para cada DrawObject
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### Ver también

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


