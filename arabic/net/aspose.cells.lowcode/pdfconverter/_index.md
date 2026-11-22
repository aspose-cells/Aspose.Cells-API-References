---
title: "الفئة PdfConverter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.LowCode.PdfConverter فئة. محول لتحويل ملف القالب إلى pdf"
type: docs
url: /ar/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

محول لتحويل ملف القالب إلى PDF.

```csharp
public class PdfConverter
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | يقوم بتحويل ملف القالب إلى pdf |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | يقوم بتحويل ملف القالب المحدد إلى pdf. |

### أمثلة

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // تهيئة PdfConverter باستخدام القالب ومسارات الإخراج
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


