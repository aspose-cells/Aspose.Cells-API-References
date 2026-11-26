---
title: "DrawObjectEventHandler.Draw"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DrawObjectEventHandler. Реализует этот интерфейс для получения DrawObject и Bound при рендеринге"
type: docs
url: /ru/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

Реализуйте этот интерфейс, чтобы получить DrawObject и Bound при рендеринге.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject будет инициализирован и возвращён при рендеринге |
| x | Single | Левая позиция DrawObject |
| y | Single | Верхняя позиция DrawObject |
| ширина | Single | Ширина DrawObject |
| высота | Single | Высота DrawObject |

### Примеры

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
                // Эта реализация будет вызываться во время рендеринга для каждого DrawObject
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### См. также

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


