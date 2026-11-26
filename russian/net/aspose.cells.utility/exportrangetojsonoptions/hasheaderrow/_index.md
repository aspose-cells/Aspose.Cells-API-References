---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportRangeToJsonOptions. Указывает, содержит ли диапазон строку заголовка"
type: docs
url: /ru/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Указывает, содержит ли диапазон строку заголовка.

```csharp
public bool HasHeaderRow { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерные данные заголовками
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Создать диапазон для экспорта
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Создать экземпляр ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Отобразить текущее значение HasHeaderRow (по умолчанию false)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // Установить HasHeaderRow в true
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Экспортировать в JSON с заголовками
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Установить HasHeaderRow в false
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Экспортировать в JSON без заголовков
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Сохраните книгу
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


