---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться."
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

Если параметр OnePagePerSheet установлен в true, всё содержимое одного листа будет выводиться на одну страницу в результате. Формат бумаги из настройки pagesetup будет недействительным, а остальные настройки pagesetup сохранят своё действие.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Добавьте некоторые образцы данных в оба листа
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // Установите параметры сохранения PDF с OnePagePerSheet
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Сохраните книгу в PDF
            workbook.Save("output.pdf", options);
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


