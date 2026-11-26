---
title: "Класс ExportRangeToJsonOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Utility.ExportRangeToJsonOptions класс. Указывает параметры, используемые при экспорте диапазона в JSON"
type: docs
url: /ru/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Указывает параметры экспорта диапазона в JSON.

```csharp
public class ExportRangeToJsonOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Экспортирует строковое значение ячеек в JSON. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Указывает, экспортировать ли пустые ячейки как null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Указывает, содержит ли диапазон строку заголовка. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Указывает отступ. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте параметры экспорта
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Экспортировать диапазон в JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // Вывести JSON
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // Сохранить в файл (необязательно)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


