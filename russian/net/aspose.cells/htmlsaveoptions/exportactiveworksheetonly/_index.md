---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли только активный лист в файл html. Если true, то будет экспортирован только активный лист в файл html. Если false, то будет экспортирована вся книга в файл html. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Указывает, экспортировать ли только активный лист в HTML‑файл. Если true, будет экспортирован только активный лист; если false — будет экспортирована вся рабочая книга. Значение по умолчанию — false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // Создать новую книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Добавить примерные данные на оба листа
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Установить параметры сохранения HTML для экспорта только активного листа
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Установить первый лист активным
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Сохранить только с активным листом
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Изменить активный лист и сохранить снова
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


