---
title: "Enum PrintingPageType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PrintingPageType enum. Hangi sayfaların yazdırılmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Hangi sayfaların yazdırılmayacağını gösterir.

```csharp
public enum PrintingPageType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Tüm sayfaları yazdırır. |
| IgnoreBlank | `1` | Hücrelerin boş olduğu sayfaları yazdırma. |
| IgnoreStyle | `2` | Hücrelerin yalnızca stil içerdiği sayfaları yazdırma. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // PdfSaveOptions oluştur
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // PrintingPageType'ı IgnoreBlank olarak ayarla
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Çalışma kitabını belirtilen seçeneklerle PDF olarak kaydet
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // PrintingPageType'ı IgnoreStyle olarak ayarla
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Çalışma kitabını belirtilen seçeneklerle PDF olarak kaydet
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // PrintingPageType'ı Default olarak ayarla
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Çalışma kitabını belirtilen seçeneklerle PDF olarak kaydet
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


