---
title: "DrawObjectEventHandler.Draw"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DrawObjectEventHandler yöntemi. Bu arayüzü, oluşturma sırasında DrawObject ve Bound elde etmek için uygular"
type: docs
url: /tr/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Renderleme sırasında DrawObject ve Bound elde etmek için bu arabirimi uygular.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject, oluşturma sırasında başlatılacak ve döndürülecek |
| x | Single | DrawObject'in sol konumu |
| y | Single | DrawObject'in üst konumu |
| genişlik | Single | DrawObject'in genişliği |
| yükseklik | Single | DrawObject'in yüksekliği |

### Örnekler

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
                // Bu uygulama, her DrawObject için oluşturma sırasında çağrılacak
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


