---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptions. تحصل وتعيّن صيغة الحفظ للمخرجات. عادةً في عملية محددة بطريقة منخفضة الكود يُسمح فقط ببعض الصيغ المحددة. يرجى تحديد الصيغة الصحيحة للعملية المقابلة وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء."
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

الحصول وتعيين تنسيق الحفظ للإخراج. عادةً، في عمليات محددة بطريقة منخفضة الكود، يُسمح فقط ببعض الصيغ المحددة. يرجى تحديد الصيغة الصحيحة للعملية المقابلة، وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // تهيئة LowCodeSaveOptions بصيغ مختلفة
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // تكوين خيارات حفظ Excel
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // تكوين خيارات حفظ PDF
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // إظهار حفظ الصيغة الأصلية
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // إظهار تغيير الصيغة وإعادة الحفظ
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


