---
title: "ExternalLink.DataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLink. Представляет источник данных внешней ссылки"
type: docs
url: /ru/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Представляет источник данных внешней ссылки.

```csharp
public string DataSource { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте внешнюю ссылку на другую книгу
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить внешние ссылки
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Получите доступ к свойству DataSource внешней ссылки
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### См. также

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


