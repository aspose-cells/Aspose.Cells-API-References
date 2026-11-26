---
title: "HtmlSaveOptions.ExportWorksheetCSSSeparately"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, следует ли экспортировать CSS листа отдельно. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Указывает, экспортировать ли CSS листа отдельно.Значение по умолчанию — false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetCSSSeparatelyDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Установите параметры сохранения HTML с ExportWorksheetCSSSeparately
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportWorksheetCSSSeparately = true;
            
            // Сохраните книгу в формате HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with separate CSS saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


