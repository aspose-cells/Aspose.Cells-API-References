---
title: "PdfSaveOptions.Bookmark"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. PdfBookmarkEntry nesnesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

[`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/) nesnesini alır ve ayarlar.

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyBookmarkDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Üç çalışma sayfası ekle
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // Yer imi hedefi olacak hücrelerdeki değerleri ayarlayın
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // Kök yer imini oluşturun
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // Alt yer imleri oluşturun
            PdfBookmarkEntry subBookmark1 = new PdfBookmarkEntry
            {
                Text = "Sheet2",
                Destination = sheet2.Cells["A1"]
            };

            PdfBookmarkEntry subBookmark2 = new PdfBookmarkEntry
            {
                Text = "Sheet3",
                Destination = sheet3.Cells["A1"]
            };

            // Alt yer imlerini köke ekleyin
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // Yer imleriyle PDF kaydetme seçeneklerini yapılandırın
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // Bellek akışına kaydedin (gerçek kullanımda dosyaya kaydedilebilir)
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


