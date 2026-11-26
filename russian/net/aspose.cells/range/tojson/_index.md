---
title: "Range.ToJson"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Преобразовать диапазон в значение JSON"
type: docs
url: /ru/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Преобразовать диапазон в значение JSON.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | JsonSaveOptions | Опции преобразования |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToJsonWithJsonSaveOptionsDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            
            // Пример данных
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);

            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


