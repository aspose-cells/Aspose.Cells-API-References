---
title: "Класс ReplaceOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ReplaceOptions. Представляет параметры замены"
type: docs
url: /ru/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Представляет параметры замены.

```csharp
public class ReplaceOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Указывает, чувствителен ли искомый строк к регистру. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | Настройки богатого форматирования для заменённого текста. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Указывает, следует ли сопоставлять полное содержимое ячеек |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Указывает, является ли искомый ключ регулярным выражением. Если true, то искомый ключ будет рассматриваться как regex. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Получает и задаёт флаги применения настроек шрифта. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Создать ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Заменить "Hello" на "Hi" в листе
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Вывести количество выполненных замен.
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Сохраните книгу
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


