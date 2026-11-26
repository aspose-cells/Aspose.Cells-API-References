---
title: "ReplaceOptions.MatchEntireCellContents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ReplaceOptions свойство. Указывает, следует ли сопоставлять содержимое целых ячеек"
type: docs
url: /ru/net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

Указывает, следует ли сопоставлять полное содержимое ячеек

```csharp
public bool MatchEntireCellContents { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyMatchEntireCellContentsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить образцы значений ячеек
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("apple pie");
            worksheet.Cells["A3"].PutValue("an apple");
            worksheet.Cells["A4"].PutValue("apples");

            // Заменить с MatchEntireCellContents = true (только точное совпадение)
            ReplaceOptions options1 = new ReplaceOptions();
            options1.MatchEntireCellContents = true;
            workbook.Replace("apple", "orange", options1);

            // Заменить с MatchEntireCellContents = false (частичное совпадение)
            ReplaceOptions options2 = new ReplaceOptions();
            options2.MatchEntireCellContents = false;
            workbook.Replace("apple", "banana", options2);

            // Вывести результаты
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue); // orange (exact match)
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // banana pie (partial match)
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // an banana (partial match)
            Console.WriteLine("A4: " + worksheet.Cells["A4"].StringValue); // bananas (partial match)
        }
    }
}
```

### См. также

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


