---
title: "Cell.Replace"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Заменить текст ячейки с параметрами"
type: docs
url: /ru/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Заменить текст ячейки с параметрами.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | String | Строковое значение для замены |
| опции | ReplaceOptions | Параметры замены |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Создать параметры замены
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // Получить настройки шрифта из ячейки B1 для применения к заменам
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Заменить все варианты "hello" на "Hi", используя параметры
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


