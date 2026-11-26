---
title: "PdfBookmarkEntry.Destination"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfBookmarkEntry. Ячейка, к которой ведет ссылка закладки"
type: docs
url: /ru/net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

Ячейка, к которой привязана ссылка закладки.

```csharp
public Cell Destination { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyDestinationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерное содержимое
            worksheet.Cells["A1"].PutValue("Bookmark Destination");
            
            // Настроить параметры сохранения PDF с закладкой
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Sample Bookmark";
            entry.Destination = worksheet.Cells["A1"]; // Demonstrate Destination property
            entry.IsOpen = true;
            
            pdfSaveOptions.Bookmark = entry;
            
            // Сохранить PDF
            workbook.Save("PdfBookmarkEntryPropertyDestinationDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


