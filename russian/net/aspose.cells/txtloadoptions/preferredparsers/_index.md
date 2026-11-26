---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Получает и задает предпочтительные парсеры значений для загрузки текстового файла"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Получает и задаёт предпочтительные парсеры значений для загрузки текстового файла.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Примечания

parsers[0] — это парсер, который будет использоваться для первого столбца в файле шаблона текста, parsers[1] — это парсер, который будет использоваться для второго столбца, … и т.д. Последний (parsers[parsers.length-1]) будет использоваться для всех остальных столбцов, начиная с parsers.length-1. Если один элемент равен null, соответствующий столбец будет разобран парсером по умолчанию из Aspose.Cells.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // Создать параметры загрузки CSV
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Установите предпочтительные парсеры — сначала попробуйте пользовательский строковый парсер, затем парсеры по умолчанию
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Пример CSV-данных с датами
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Загрузить книгу с параметрами
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Проверьте результаты парсинга
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### См. также

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


