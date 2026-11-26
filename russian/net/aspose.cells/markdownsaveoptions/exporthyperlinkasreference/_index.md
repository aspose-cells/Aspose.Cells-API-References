---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Указывает, следует ли экспортировать гиперссылку с использованием определений ссылок вместо встроенного формата. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Указывает, экспортировать ли гиперссылку с использованием определений ссылок вместо встроенного формата. Значение по умолчанию — false.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Поместите примерный текст в ячейку
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Добавьте гиперссылку в ячейку (A1)
            // Параметры: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Инициализируйте параметры сохранения Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Непосредственно обратитесь к свойству ExportHyperlinkAsReference (только для чтения в этой демонстрации)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Сохраните книгу в формате markdown; свойство (если true) будет влиять на то, как экспортируются гиперссылки
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


