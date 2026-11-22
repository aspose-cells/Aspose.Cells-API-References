---
title: "Enum PdfCompliance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Rendering.PdfCompliance enum. يسمح للمستخدم بتعيين توافق تحويلات PDF"
type: docs
url: /ar/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

السماح للمستخدم بتعيين توافق تحويل PDF.

```csharp
public enum PdfCompliance
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | تنسيق PDF متوافق مع PDF 1.4 |
| Pdf14 | `0` | تنسيق PDF متوافق مع PDF 1.4 |
| Pdf15 | `3` | تنسيق PDF متوافق مع PDF 1.5 |
| Pdf16 | `4` | تنسيق PDF متوافق مع PDF 1.6 |
| Pdf17 | `5` | تنسيق PDF متوافق مع PDF 1.7 |
| PdfA1b | `1` | تنسيق PDF متوافق مع PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | تنسيق PDF متوافق مع PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | تنسيق PDF متوافق مع PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | تنسيق PDF متوافق مع PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | تنسيق PDF متوافق مع PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | تنسيق PDF متوافق مع PDF/A-3b (ISO 19005-3) |
| PdfA3u | `10` | تنسيق PDF متوافق مع PDF/A-3u (ISO 19005-3) |
| PdfA3a | `11` | تنسيق PDF متوافق مع PDF/A-3a (ISO 19005-3) |

### أمثلة

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
            // إنشاء دفتر عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // تعيين خيارات حفظ PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // تعيين مستوى الامتثال إلى PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // حفظ دفتر العمل إلى PDF بالمستوى المحدد للامتثال
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


