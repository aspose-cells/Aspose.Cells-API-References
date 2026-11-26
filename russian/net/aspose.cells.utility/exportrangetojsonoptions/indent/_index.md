---
title: "ExportRangeToJsonOptions.Indent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportRangeToJsonOptions. Указывает отступ"
type: docs
url: /ru/net/aspose.cells.utility/exportrangetojsonoptions/indent/
---
## ExportRangeToJsonOptions.Indent property

Указывает отступ.

```csharp
public string Indent { get; set; }
```

### Примечания

Если отступ равен null или пуст, экспортированный json не будет отформатирован.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать экземпляр ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Отобразить текущий отступ (по умолчанию null)
            Console.WriteLine("Current Indent value: " + (options.Indent ?? "null"));

            // Экспортировать с отступом по умолчанию (компактный JSON)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
            string jsonWithoutIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without indent:\n" + jsonWithoutIndent);

            // Установить отступ в 4 пробела
            options.Indent = "    ";
            string jsonWithIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with 4-space indent:\n" + jsonWithIndent);

            // Установить отступ табуляцией
            options.Indent = "\t";
            string jsonWithTabIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with tab indent:\n" + jsonWithTabIndent);
        }
    }
}
```

### См. также

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


