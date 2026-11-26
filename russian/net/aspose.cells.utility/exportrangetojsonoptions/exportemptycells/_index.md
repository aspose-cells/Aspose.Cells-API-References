---
title: "ExportRangeToJsonOptions.ExportEmptyCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportRangeToJsonOptions. Указывает, экспортировать ли пустые ячейки как null"
type: docs
url: /ru/net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

Указывает, экспортировать ли пустые ячейки как null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            // Оставить B2 пустой намеренно
            
            // Создать параметры экспорта и включить экспорт пустых ячеек
            ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
            exportOptions.ExportEmptyCells = true;
            
            // Экспортировать диапазон в JSON
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            
            Console.WriteLine(jsonData);
        }
    }
}
```

### См. также

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


