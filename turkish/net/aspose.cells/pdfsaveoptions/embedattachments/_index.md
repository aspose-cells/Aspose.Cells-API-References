---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Excel'deki Ole nesneleri için ekin gömülüp gömülmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Excel'deki Ole nesneleri için ekleri gömmeyi gösterir.

```csharp
public bool EmbedAttachments { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur. PDF/A uyumluluğu ayarlandığında veya pdf şifrelemesi etkinleştirildiğinde değer false olmalıdır.

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Gömme için örnek bir dosya oluşturun
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Çalışma sayfasına bir ek (OLE nesnesi) ekleyin
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // EmbedAttachments özelliğini true olarak ayarlayın
            pdfSaveOptions.EmbedAttachments = true;

            // Çalışma kitabını gömülü eklerle PDF olarak kaydedin
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Temizle
            File.Delete(sampleFile);
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


