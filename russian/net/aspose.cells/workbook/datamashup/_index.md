---
title: "Workbook.DataMashup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает данные mashup"
type: docs
url: /ru/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Получает данные mashup.

```csharp
public DataMashup DataMashup { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пример данных для запуска Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // Сохранить в файл
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // Повторно откройте книгу, чтобы получить доступ к DataMashup
            workbook = new Workbook(sourcePath);
            
            // Получите доступ к формулам Power Query через свойство DataMashup
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Выведите базовую информацию о запросах
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // Если есть запросы, покажите детали первого из них
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // Сохранить в новый файл
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### См. также

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


