---
title: "DigitalSignature.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. تحدد GUID يمكن الإشارة إليه مع GUID لخط التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty جميع الأصفار Guid"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

يحدد GUID يمكن الإشارة إليه عبره مع GUID لخط التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty (جميع الأصفار) Guid.

```csharp
public Guid Id { get; set; }
```

### ملاحظات

عند الضبط، يربط [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) بـ [`DigitalSignature`](../).

### أمثلة

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء توقيع رقمي بمعرف محدد
            Guid signatureId = Guid.NewGuid();
            
            // أنشئ توقيعًا رقميًا
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // تعيين معرف التوقيع
            signature.Id = signatureId;

            // إضافة توقيع إلى المجموعة
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // تطبيق التوقيع الرقمي على المصنف
            workbook.SetDigitalSignature(dsCollection);

            // احفظ المصنف
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


