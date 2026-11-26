---
title: "ReplaceOptions.RegexKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReplaceOptions. Указывает, является ли искомый ключ регулярным выражением. Если true, то искомый ключ будет рассматриваться как regex"
type: docs
url: /ru/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Указывает, является ли искомый ключ регулярным выражением. Если true, то искомый ключ будет рассматриваться как regex.

```csharp
public bool RegexKey { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Создать книгу с образцовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Создать параметры замены с regex
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // Заменить все слова, начинающиеся с 'p' или 'b', за которыми следует гласная
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Выполнить замену
            workbook.Replace(pattern, replacement, options);

            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


