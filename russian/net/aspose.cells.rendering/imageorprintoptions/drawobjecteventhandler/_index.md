---
title: "ImageOrPrintOptions.DrawObjectEventHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Реализует этот интерфейс для получения DrawObject и Bound при рендеринге"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Реализуйте этот интерфейс, чтобы получить DrawObject и Bound при рендеринге.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Примеры

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
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Создайте пользовательский обработчик события DrawObject
            var drawHandler = new CustomDrawObjectEventHandler();

            // Установите параметры изображения с помощью обработчика событий
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DrawObjectEventHandler = drawHandler;

            // Отрендерьте лист, чтобы вызвать события
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
            // Пример: Выведите информацию о нарисованном объекте
            Console.WriteLine($"Drawing {drawObject.Type} at ({x},{y}) with size {width}x{height}");
        }
    }
}
```

### См. также

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


