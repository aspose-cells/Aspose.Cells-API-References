---
title: "JsonLayoutOptions.DateFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Получает и задает формат значения даты"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

Получает и задает формат значения даты.

```csharp
public string DateFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Настроить параметры импорта JSON с пользовательским форматом даты
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "DD-MM-YYYY";

            // Импортировать данные JSON с датами
            string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            // Проверить, что дата была импортирована с правильным форматом
            Cell dateCell = worksheet.Cells["A2"];
            Console.WriteLine("Imported date value: " + dateCell.StringValue);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


