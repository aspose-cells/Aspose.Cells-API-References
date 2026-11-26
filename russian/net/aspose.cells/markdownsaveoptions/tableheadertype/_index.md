---
title: "MarkdownSaveOptions.TableHeaderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Получает и задает способ установки заголовка таблицы"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/tableheadertype/
---
## MarkdownSaveOptions.TableHeaderType property

Получает и задает способ установки заголовка таблицы.

```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Создайте MarkdownSaveOptions и задайте TableHeaderType
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;

            // Сохраните как markdown с указанными параметрами
            workbook.Save("output.md", saveOptions);
        }
    }
}
```

### См. также

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


