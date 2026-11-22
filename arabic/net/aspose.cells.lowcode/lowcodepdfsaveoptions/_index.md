---
title: "فئة LowCodePdfSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.LowCode.LowCodePdfSaveOptions. خيارات حفظ PDF بطريقة منخفضة الكود"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

خيارات حفظ pdf بطريقة منخفضة الكود.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | الحصول وتعيين الملف (مع المسار إذا لزم) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [`OutputStream`](../lowcodesaveoptions/outputstream/). (موروث من [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | الحصول وتعيين الدفق لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل [`OutputFile`](../lowcodesaveoptions/outputfile/). (موروث من [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | الخيارات لحفظ ملف PDF. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | تنسيق الحفظ للإخراج. للتحويل إلى PDF، لا يمكن أن يكون إلا PDF. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // إنشاء خيارات حفظ PDF منخفضة الكود
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // احفظ باستخدام خيارات منخفضة الكود
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


