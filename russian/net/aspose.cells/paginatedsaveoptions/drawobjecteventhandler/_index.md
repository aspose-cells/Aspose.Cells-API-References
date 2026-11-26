---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Реализует этот интерфейс для получения DrawObject и Bound при рендеринге"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Реализуйте этот интерфейс, чтобы получить DrawObject и Bound при рендеринге.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных и фигур
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Создайте экземпляр параметров сохранения с пагинацией
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Отобразите текущее значение свойства (по умолчанию должно быть null)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Установите новый пользовательский обработчик события
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Это вызовет метод Draw во время рендеринга
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Измените обработчик события на null, чтобы продемонстрировать разницу
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### См. также

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


