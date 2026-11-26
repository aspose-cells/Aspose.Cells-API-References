---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Указывает, следует ли встраивать вложения для объектов Ole в Excel"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Указывает, следует ли встраивать вложения для объектов Ole в Excel.

```csharp
public bool EmbedAttachments { get; set; }
```

### Примечания

Значение по умолчанию — false. Значение должно быть false, когда включено соответствие PDF/A или включено шифрование PDF.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
using System.IO;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedAttachmentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Создать пример файла для встраивания
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Добавить вложение (OLE‑объект) в лист
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Установить свойство EmbedAttachments в true
            pdfSaveOptions.EmbedAttachments = true;

            // Сохранить книгу в формате PDF с встроенными вложениями
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Очистить
            File.Delete(sampleFile);
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


