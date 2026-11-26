---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Указывает, должно ли окно заголовка Windows отображать заголовок документа"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Указывает, должно ли заголовок окна отображать название документа.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Примечания

Если false, строка заголовка должна вместо этого отображать имя PDF‑файла. Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Установить свойство DisplayDocTitle в true
            pdfSaveOptions.DisplayDocTitle = true;

            // Сохранить книгу в формате PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


