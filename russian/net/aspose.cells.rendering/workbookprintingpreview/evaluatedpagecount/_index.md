---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookPrintingPreview. Оценить общее количество страниц этой рабочей книги"
type: docs
url: /ru/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Оцените общее количество страниц этой рабочей книги

```csharp
public int EvaluatedPageCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Создать параметры предварительного просмотра печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Создать предварительный просмотр печати рабочей книги
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Получить и отобразить оцененное количество страниц
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### См. также

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


