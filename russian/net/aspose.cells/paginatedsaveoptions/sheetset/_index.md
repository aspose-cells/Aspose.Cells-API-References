---
title: "PaginatedSaveOptions.SheetSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге (Visible)"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Создать новую книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Установите некоторые примерные данные в обоих листах
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Сохраните только второй лист, используя SheetSet
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // Сохраните книгу с указанными листами
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


