---
title: "FindOptions.ValueTypeSensitive"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Указывает, должен ли тип значения ячейки совпадать с типом искомого ключа"
type: docs
url: /ru/net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

Указывает, должен ли тип значения искомой ячейки совпадать с типом искомого ключа.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyValueTypeSensitiveDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте разные типы значений в ячейки
            worksheet.Cells["A1"].PutValue("100"); // Stored as string
            worksheet.Cells["A2"].PutValue(100);   // Stored as number
            worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
            worksheet.Cells["A4"].PutValue(100.0);   // Stored as number

            // Создайте параметры поиска с ValueTypeSensitive = true
            FindOptions options = new FindOptions();
            options.ValueTypeSensitive = true;
            options.LookAtType = LookAtType.EntireContent;

            // Поиск числа 100 (строка "100" не будет найдена)
            Cell foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));

            // Поиск строки "100" (число 100 не будет найдено)
            foundCell = worksheet.Cells.Find("100", null, options);
            Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));

            // Измените на ValueTypeSensitive = false
            options.ValueTypeSensitive = false;
            
            // Теперь оба поиска найдут любую ячейку с "100" или 100
            foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


