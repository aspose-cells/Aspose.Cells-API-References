---
title: "DigitalSignature.IsValid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. إذا كان هذا التوقيع الرقمي صالحًا ولم يتم العبث بالمستند، ستكون القيمة true"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

إذا كان هذا التوقيع الرقمي صالحًا ولم يتم العبث بالمستند، ستكون هذه القيمة true.

```csharp
public bool IsValid { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System.IO;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIsValidDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بعض البيانات إلى ورقة العمل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // احفظ المصنف أولاً
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // إنشاء مجموعة توقيع رقمي
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // إنشاء توقيع رقمي (في السيناريو الحقيقي، استخدم شهادة صحيحة)
            // المعامل الأول يجب أن يكون byte[] لبيانات الشهادة
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // توقيع المصنف
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // تحقق من التوقيع
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection loadedSignatures = signedWorkbook.GetDigitalSignature();
            
            foreach (DigitalSignature sig in loadedSignatures)
            {
                Console.WriteLine("Signature is valid: " + sig.IsValid);
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


