---
title: "SheetRender.PageCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SheetRender. Возвращает общее количество страниц текущего листа"
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Получает общее количество страниц текущего листа.

```csharp
public int PageCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Установите параметры страницы для печати
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // Создайте SheetRender с параметрами по умолчанию
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Отобразите количество страниц
            Console.WriteLine("Page Count: " + render.PageCount);

            // Измените параметры страницы, чтобы принудительно создать несколько страниц
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Создайте новый SheetRender, чтобы получить обновлённое количество страниц
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


