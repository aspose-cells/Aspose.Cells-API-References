---
title: "Enum PdfCompliance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfCompliance enum. Kullanıcının PDF dönüşüm uyumluluğunu ayarlamasına izin verir"
type: docs
url: /tr/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Kullanıcının PDF dönüşümünün Uyumluluğunu ayarlamasına izin verir.

```csharp
public enum PdfCompliance
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | PDF 1.4 ile uyumlu PDF formatı |
| Pdf14 | `0` | PDF 1.4 ile uyumlu PDF formatı |
| Pdf15 | `3` | PDF 1.5 ile uyumlu PDF formatı |
| Pdf16 | `4` | PDF 1.6 ile uyumlu PDF formatı |
| Pdf17 | `5` | PDF 1.7 ile uyumlu PDF formatı |
| PdfA1b | `1` | PDF/A-1b (ISO 19005-1) ile uyumlu PDF formatı |
| PdfA1a | `2` | PDF/A-1a (ISO 19005-1) ile uyumlu PDF formatı |
| PdfA2b | `6` | PDF/A-2b (ISO 19005-2) ile uyumlu PDF formatı |
| PdfA2u | `7` | PDF/A-2u (ISO 19005-2) ile uyumlu PDF formatı |
| PdfA2a | `8` | PDF/A-2a (ISO 19005-2) ile uyumlu PDF formatı |
| PdfA3b | `9` | PDF/A-3b (ISO 19005-3) ile uyumlu PDF formatı |
| PdfA3u | `10` | PDF/A-3u (ISO 19005-3) ile uyumlu PDF formatı |
| PdfA3a | `11` | PDF/A-3a (ISO 19005-3) ile uyumlu PDF formatı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfComplianceDemo
    {
        public static void PdfComplianceExample()
        {
            // Bir çalışma kitabı oluşturma
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // PDF kaydetme seçeneklerini ayarlama
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Uyumluluk seviyesini PDF/A-1b olarak ayarlama
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Belirtilen uyumluluk seviyesiyle çalışma kitabını PDF olarak kaydetme
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


