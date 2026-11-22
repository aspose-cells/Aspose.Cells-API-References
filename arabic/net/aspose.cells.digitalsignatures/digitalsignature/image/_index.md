---
title: "DigitalSignature.Image"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. تحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

يحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null.

```csharp
public byte[] Image { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.DigitalSignatures;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyImageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // إضافة خط توقيع إلى ورقة العمل
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // إنشاء شهادة اختبار (في الاستخدام الحقيقي، تحميل من ملف)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // إنشاء توقيع رقمي مع صورة
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // إضافة التوقيع وحفظ
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // حفظ إلى تدفق الذاكرة
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


