---
title: "WorkbookRender.WorkbookRender"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор WorkbookRender. Конструирование WorkbookRender"
type: docs
url: /ru/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

Конструкция WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| рабочая книга | Рабочая книга | Указать, какую книгу следует отрендерить. |
| опции | ImageOrPrintOptions | ImageOrPrintOptions содержит некоторые свойства выходного изображения |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Создать параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Создать рендерер книги
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Вывести количество страниц
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### См. также

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


