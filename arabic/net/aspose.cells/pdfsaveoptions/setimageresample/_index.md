---
title: "PdfSaveOptions.SetImageResample"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PdfSaveOptions. تعيين PPIpixels المطلوب لكل بوصة لإعادة تحجيم الصور وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG باستخدام إعداد الجودة المحدد وستتم إعادة تحجيم الصور التي تتجاوز PPIpixels المحدد لكل بوصة."
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

يضبط قيمة PPI (بكسل لكل بوصة) المطلوبة لإعادة تحجيم الصور وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG باستخدام إعداد الجودة المحدد، وستتم إعادة تحجيم الصور التي تتجاوز قيمة PPI المحددة (بكسل لكل بوصة).

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredPPI | Int32 | البكسلات المطلوبة لكل بوصة. 220 جودة عالية. 150 جودة الشاشة. 96 جودة البريد الإلكتروني. |
| jpegQuality | Int32 | 0 - 100% جودة JPEG. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodSetImageResampleWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("Book1.xlsx");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.SetImageResample(96, 80);
            
            wb.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


