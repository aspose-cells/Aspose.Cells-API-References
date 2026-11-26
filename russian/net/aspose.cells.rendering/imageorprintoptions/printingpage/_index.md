---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает, какие страницы не будут печататься"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Указывает, какие страницы не будут печататься.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintingPageDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // Создать параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // Отобразить книгу с указанными параметрами
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // Вывести количество страниц (будут игнорироваться пустые страницы)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // Переключиться на поведение по умолчанию (включать все страницы)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### См. также

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


