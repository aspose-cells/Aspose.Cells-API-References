---
title: "DrawObject.SheetIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DrawObject. Указывает текущий индекс листа DrawObject"
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

Указывает текущий индекс листа DrawObject.

```csharp
public int SheetIndex { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // Пользовательский обработчик, который считывает и отображает SheetIndex каждого DrawObject
    class SheetIndexReaderHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
            Console.WriteLine($"Page: {drawObject.CurrentPage + 1}/{drawObject.TotalPages}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
            Console.WriteLine();
        }
    }

    public class DrawObjectPropertySheetIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Заполните несколько ячеек, чтобы иметь содержимое для рендеринга
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Добавьте фигуру, чтобы объекты отрисовки фигур также генерировались
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Настройте параметры рендеринга с нашим пользовательским обработчиком
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // Выполните рендеринг листа – это вызывает события DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // Сохраните книгу (необязательно)
                workbook.Save("SheetIndexDemo.xlsx");
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


