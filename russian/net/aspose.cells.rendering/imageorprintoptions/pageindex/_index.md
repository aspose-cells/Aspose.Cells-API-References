---
title: "ImageOrPrintOptions.PageIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает нулевой индекс первой сохраняемой страницы"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

Получает или задает нулевой индекс первой страницы для сохранения.

```csharp
public int PageIndex { get; set; }
```

### Примечания

По умолчанию 0.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные на несколько страниц
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            // Настроить параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PageIndex = 1; // Start from second page (0-based index would be 1)
            options.PageCount = 1; // Only process one page

            // Создать рендер листа для первого рабочего листа
            SheetRender render = new SheetRender(worksheet, options);

            // Сохранить в PDF, используя правильный метод API
            render.ToImage(0, "output.pdf");
            Console.WriteLine("Saved page 2 to PDF successfully.");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


