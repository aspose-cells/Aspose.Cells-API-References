---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Указывает, экспортировать ли скрытое содержимое листа.Значение по умолчанию — true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // Установите параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // Сохранить без экспорта скрытого листа
            workbook.Save("output_without_hidden.html", saveOptions);

            // Изменить параметр для экспорта скрытых листов
            saveOptions.ExportHiddenWorksheet = true;

            // Сохранить с экспортом скрытого листа
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


