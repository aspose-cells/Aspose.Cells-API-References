---
title: "DrawObject.Shape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DrawObject. Указывает объект Shape при рендеринге. Доступны все свойства фигуры."
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/shape/
---
## DrawObject.Shape property

Указывает объект Shape при рендеринге. Все свойства фигуры доступны.

```csharp
public Shape Shape { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyShapeDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте примерные данные, чтобы сделать рендеринг осмысленным
                worksheet.Cells["A1"].Value = "Sample Data";
                worksheet.Cells["A2"].Value = "More Data";

                // Добавить форму на лист
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Настройте параметры рендеринга с пользовательским обработчиком
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new ShapePropertyHandler()
                };

                // Выполните рендеринг листа - это вызовет события DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "ShapeDemo.png");

                // Сохраните книгу
                workbook.Save("ShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Пользовательский обработчик для захвата событий DrawObject и чтения свойства Shape
        private class ShapePropertyHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Shape != null)
                {
                    Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                    Console.WriteLine($"Shape Name: {drawObject.Shape.Name}");
                    Console.WriteLine($"Shape Text: {drawObject.Shape.Text}");
                    Console.WriteLine($"Shape Width: {drawObject.Shape.Width} pixels");
                    Console.WriteLine($"Shape Height: {drawObject.Shape.Height} pixels");
                    Console.WriteLine($"Shape Type: {drawObject.Shape.AutoShapeType}");
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### См. также

* class [Shape](../../../aspose.cells.drawing/shape/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


