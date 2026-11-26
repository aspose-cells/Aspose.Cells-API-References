---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Указывает, какие страницы не будут печататься"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Указывает, какие страницы не будут печататься.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Примечания

Если содержимое листа разреженное, в результирующем PDF‑файле могут появиться полностью пустые страницы. Если вы не хотите этих пустых страниц, можете использовать эту опцию для их исключения.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Создать пустой лист
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Сохранить, игнорируя пустые страницы
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Сохранить, игнорируя пустые страницы и страницы только со стилем
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


