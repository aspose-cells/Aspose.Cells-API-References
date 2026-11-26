---
title: "Workbook.FileName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает и задает текущее имя файла"
type: docs
url: /ru/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Получает и задает текущее имя файла.

```csharp
public string FileName { get; set; }
```

### Примечания

Если файл открыт через поток и есть внешние ссылки на формулы, пожалуйста, задайте имя файла.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Задайте свойство имени файла
            wb.FileName = "SampleWorkbook.xlsx";
            
            // Добавьте некоторые данные для демонстрации функциональности
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Сохраните книгу
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Продемонстрировать изменение имени файла
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Продемонстрировать использование внешних ссылок
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


