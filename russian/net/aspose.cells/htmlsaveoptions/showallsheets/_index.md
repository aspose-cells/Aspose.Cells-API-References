---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, показывать ли все листы при сохранении в один HTML‑файл."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Указывает, показывать ли все листы при сохранении в один HTML‑файл.

```csharp
public bool ShowAllSheets { get; set; }
```

### Примечания

Работает только когда [`SaveAsSingleFile`](../saveassinglefile/) равно True.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с несколькими листами.
            Workbook workbook = new Workbook();
            
            // Добавьте данные на первый лист.
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // Добавьте второй лист.
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Добавьте третий лист.
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установите свойство ShowAllSheets в true, чтобы экспортировать все листы.
            saveOptions.ShowAllSheets = true;

            // Сохранить книгу с отображением всех листов в HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


