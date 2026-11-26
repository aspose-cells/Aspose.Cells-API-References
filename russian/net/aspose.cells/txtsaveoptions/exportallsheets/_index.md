---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Указывает, следует ли экспортировать все листы в текстовый файл. Если false, экспортируется только активный лист, как в MS Excel"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Указывает, экспортировать ли все листы в текстовый файл. Если false, экспортируется только активный лист, как в MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // Создайте книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Добавить примерные данные на оба листа
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // Сохраните с ExportAllSheets=false (по умолчанию)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // Сохраните с ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


