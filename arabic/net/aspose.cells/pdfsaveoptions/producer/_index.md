---
title: "PdfSaveOptions.Producer"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل وتعيّن المنتج لمستند PDF المُنشأ"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

يحصل على ويضبط المنتج للمستند PDF المُنشأ.

```csharp
public string Producer { get; set; }
```

### ملاحظات

إذا كانت القيمة فارغة (null)، أو لم يتم تعيين رخصة صالحة (LICENSE)، فسيتم استخدام السلسلة Aspose.Cells vVERSION.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyProducerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // عيّن خاصية Producer
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // حفظ إلى تدفق الذاكرة
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // تحقق من تعيين Producer
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)") 
                        ? "Producer property set successfully" 
                        : "Failed to set Producer property");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


