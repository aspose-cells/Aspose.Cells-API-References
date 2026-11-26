---
title: "DrawObject.CurrentPage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DrawObject. Указывает индекс страницы DrawObject. Индекс страницы начинается с нуля. Один лист содержит несколько страниц при рендеринге"
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Указывает индекс страницы DrawObject. Индекс страницы начинается с нуля. Один лист содержит несколько страниц при рендеринге.

```csharp
public int CurrentPage { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // Пользовательский обработчик для чтения и отображения свойства CurrentPage
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Отобразить значение свойства CurrentPage
                Console.WriteLine($"CurrentPage: {drawObject.CurrentPage}");
                Console.WriteLine($"TotalPages: {drawObject.TotalPages}");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Создать новую книгу и получить доступ к первому листу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте некоторые примерные данные, чтобы сделать рендеринг осмысленным
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Добавьте фигуру, чтобы генерировать объекты отрисовки типа shape
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Настройте параметры рендеринга с нашим пользовательским обработчиком отрисовки
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Отобразите лист, чтобы вызвать события DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Сохраните книгу
                workbook.Save("CurrentPageDemo.xlsx");
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


