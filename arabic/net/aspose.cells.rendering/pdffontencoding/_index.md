---
title: "تعداد PdfFontEncoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.PdfFontEncoding. يمثل ترميز الخط المضمن في PDF"
type: docs
url: /ar/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

يمثل ترميز الخط المدمج في PDF.

```csharp
public enum PdfFontEncoding
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Identity | `0` | يمثل استخدام ترميز Identity-H لجميع الخطوط المضمنة في PDF. |
| AnsiPrefer | `1` | يمثل التفضيل لاستخدام WinAnsiEncoding للخطوط TrueType التي تحتوي على الأحرف 32-127، وإلا سيُستخدم ترميز Identity-H للخطوط المضمنة في PDF. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // أنشئ PdfSaveOptions وعيّن خاصية FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // حفظ المصنف كملف PDF
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


