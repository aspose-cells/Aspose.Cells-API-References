---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Указывает, экспортировать ли свойства листа.Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Установить параметры сохранения HTML с отключённым ExportWorksheetProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Сохранить с отключёнными свойствами листа
            workbook.Save("output_without_worksheet_props.html", options);

            // Включить экспорт свойств листа
            options.ExportWorksheetProperties = true;
            
            // Сохранить с включёнными свойствами листа
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


