---
title: "Перечисление MarkdownTableHeaderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Markdown.MarkdownTableHeaderType. Представляет тип заголовка таблицы в markdown‑файле"
type: docs
url: /ru/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Представляет тип заголовка таблицы в markdown-файле.

```csharp
public enum MarkdownTableHeaderType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| FirstRow | `0` | Первая строка как заголовок таблицы. |
| ColumnHeader | `1` | Имя столбца (например A,B,C…) как заголовок таблицы. |
| Empty | `2` | Пустая строка заголовка. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Установить параметры сохранения Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Сохранить как файл Markdown
            workbook.Save("output.md", saveOptions);
            
            // Проверьте вывод
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


