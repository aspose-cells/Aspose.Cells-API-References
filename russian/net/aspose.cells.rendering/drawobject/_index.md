---
title: "Класс DrawObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.DrawObject. DrawObject будет инициализирован и возвращён при рендеринге"
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

DrawObject будет инициализирован и возвращён при рендеринге.

```csharp
public class DrawObject
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Указывает объект Cell при рендеринге. Все свойства ячейки доступны. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Указывает индекс страницы DrawObject. Индекс страницы начинается с нуля. Один лист содержит несколько страниц при рендеринге. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Указывает байты изображения отрисованного Chart, Shape при рендеринге. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Указывает объект Shape при рендеринге. Все свойства фигуры доступны. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Указывает текущий индекс листа DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Указывает общее количество страниц в текущем рендеринге. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Указывает тип DrawObject. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // Пользовательская реализация DrawObjectEventHandler
    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
    }

    public class DrawObjectDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Добавить фигуру
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // Создать экземпляр CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Установить параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Отрендерить лист в изображение
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Сохраните книгу
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


