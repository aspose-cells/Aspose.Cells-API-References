---
title: "DrawObject.TotalPages"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DrawObject. Указывает общее количество страниц в текущем рендеринге"
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Указывает общее количество страниц в текущем рендеринге.

```csharp
public int TotalPages { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyTotalPagesDemo
    {
        // Пользовательский обработчик для захвата событий DrawObject и чтения свойства TotalPages
        private class TotalPagesHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Отобразите значение свойства TotalPages
                Console.WriteLine($"Total Pages in Rendering: {drawObject.TotalPages}");
                Console.WriteLine($"Current Page: {drawObject.CurrentPage + 1}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Добавьте примерные данные, чтобы сделать рендеринг осмысленным
                sheet.Cells["A1"].PutValue("Sample Data");
                sheet.Cells["A2"].PutValue("More Data");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Добавьте форму, чтобы гарантировать генерацию нескольких draw‑объектов
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Настройте параметры рендеринга с нашим пользовательским обработчиком
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = false, // Allow multiple pages to demonstrate TotalPages
                    DrawObjectEventHandler = new TotalPagesHandler()
                };

                // Выполните рендеринг листа - это вызовет события DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "TotalPagesDemo.png");

                // Сохраните книгу
                workbook.Save("TotalPagesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


