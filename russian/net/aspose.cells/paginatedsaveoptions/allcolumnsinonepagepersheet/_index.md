---
title: "PaginatedSaveOptions.AllColumnsInOnePagePerSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина формата бумаги из настройки PageSetup будет игнорироваться, а остальные настройки PageSetup сохранят своё действие"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

Если параметр AllColumnsInOnePagePerSheet установлен в true, всё содержимое столбцов одного листа будет выводиться на одну страницу в результате. Ширина формата бумаги из настройки pagesetup будет игнорироваться, а остальные настройки pagesetup сохранят своё действие.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для демонстрации подгонки столбцов
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[0, i].PutValue("Column " + (i + 1));
                worksheet.Cells[1, i].PutValue("Sample data " + (i + 1));
            }

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;

            // Сохраните книгу с указанными параметрами
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with all columns in one page per sheet.");
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


