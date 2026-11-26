---
title: "DrawObject.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DrawObject. Указывает тип DrawObject"
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/type/
---
## DrawObject.Type property

Указывает тип DrawObject.

```csharp
public DrawObjectEnum Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    public class DrawObjectPropertyTypeDemo
    {
        // Пользовательский обработчик, который читает и отображает свойство Type каждого DrawObject
        private class TypeReaderHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}, Page: {drawObject.CurrentPage}/{drawObject.TotalPages}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Создать новую книгу и получить доступ к первому листу
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Заполните несколько ячеек
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Добавьте форму, чтобы также генерировать draw‑объекты типа shape
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Установите параметры рендеринга с нашим пользовательским draw‑обработчиком
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new TypeReaderHandler()
                };

                // Отобразите лист – это вызывает события DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectTypeDemo.png");

                // Сохраните книгу (необязательно)
                workbook.Save("DrawObjectTypeDemo.xlsx");
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

* enum [DrawObjectEnum](../../drawobjectenum/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


