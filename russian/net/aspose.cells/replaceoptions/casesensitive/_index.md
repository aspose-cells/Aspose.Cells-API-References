---
title: "ReplaceOptions.CaseSensitive"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReplaceOptions. Указывает, чувствителен ли регистр искомой строки"
type: docs
url: /ru/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Указывает, чувствителен ли искомый строк к регистру.

```csharp
public bool CaseSensitive { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Создать параметры замены с CaseSensitive = false
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // Заменить все регистронезависимые варианты "apple" на "orange"
            workbook.Replace("apple", "orange", options);

            // Вывести результаты
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Сбросить данные
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Изменить на CaseSensitive = true
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Вывести результаты
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### См. также

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


