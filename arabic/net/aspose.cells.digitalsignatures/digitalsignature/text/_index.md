---
title: "DigitalSignature.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. تحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

يحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty.

```csharp
public string Text { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء شهادة اختبار (في السيناريو الحقيقي، استخدم شهادة صالحة)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // إنشاء كائن توقيع رقمي
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // عرض القيمة الحالية للخاصية Text (القيمة الافتراضية هي empty)
            Console.WriteLine("Current Text value: " + signature.Text);

            // تعيين قيمة جديدة للخاصية Text
            signature.Text = "Approved by John Doe";

            // إنشاء مجموعة توقيعات رقمية وإضافة التوقيع إليها
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // إضافة التوقيعات الرقمية إلى المصنف
            workbook.AddDigitalSignature(signatures);

            // حفظ المصنف مع التوقيع الرقمي
            try
            {
                workbook.Save("DigitalSignatureWithText.xlsx");
                Console.WriteLine("Workbook saved with digital signature text: " + signature.Text);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error saving workbook: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


