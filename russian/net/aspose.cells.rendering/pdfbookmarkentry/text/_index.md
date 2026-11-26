---
title: "PdfBookmarkEntry.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfBookmarkEntry. Заголовок закладки"
type: docs
url: /ru/net/aspose.cells.rendering/pdfbookmarkentry/text/
---
## PdfBookmarkEntry.Text property

Заголовок закладки.

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерное содержимое
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Создать запись закладки PDF
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Section 1"; // Demonstrating Text property usage
            entry.Destination = worksheet.Cells["A1"];
            entry.IsOpen = true;
            
            // Установить параметры сохранения с закладкой
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.Bookmark = entry;
            
            // Сохранить рабочую книгу с закладкой
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF with bookmark created successfully.");
        }
    }
}
```

### См. также

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


