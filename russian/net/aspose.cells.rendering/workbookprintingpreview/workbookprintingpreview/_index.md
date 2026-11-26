---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор WorkbookPrintingPreview. Конструктор WorkbookPrintingPreview."
type: docs
url: /ru/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

Конструктор WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| рабочая книга | Рабочая книга | Укажите, какую книгу необходимо распечатать. |
| опции | ImageOrPrintOptions | ImageOrPrintOptions содержит некоторые свойства вывода |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Установите параметры печати.
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Создайте предварительный просмотр печати с книгой и параметрами.
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Отобразить количество страниц.
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### См. также

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


