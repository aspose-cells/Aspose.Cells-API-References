---
title: "DigitalSignature.ProviderId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. تحدد معرف الفئة لمزود التوقيع. القيمة الافتراضية هي Guid فارغ مكوّن من جميع الأصفار"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

يحدد معرف الفئة لمزود التوقيع. القيمة الافتراضية هي Empty (جميع الأصفار) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### ملاحظات

مزود الخدمة التشفيرية (CSP) هو وحدة برنامج مستقلة تقوم فعليًا بتنفيذ خوارزميات التشفير للمصادقة والترميز والتشفير. تحتفظ Microsoft Office بالقيمة {00000000-0000-0000-0000-000000000000} لمزود التوقيع الافتراضي، والقيمة {000CD6A4-0000-0000-C000-000000000046} لمزود التوقيع للغات شرق آسيا. يجب الحصول على GUID للمزود المثبت إضافيًا من الوثائق المرفقة مع المزود.

### أمثلة

```csharp
using System;
using System.IO;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyProviderIdDemo
    {
        public static void Run()
        {
            // إنشاء شهادة موقعة ذاتيًا
            X509Certificate2 certificate;
            using (var rsa = RSA.Create())
            {
                var request = new CertificateRequest(
                    new X500DistinguishedName("cn=AsposeTest"),
                    rsa,
                    HashAlgorithmName.SHA256,
                    RSASignaturePadding.Pkcs1);
                
                certificate = request.CreateSelfSigned(DateTimeOffset.Now, DateTimeOffset.Now.AddHours(1));
            }

            // إنشاء مصنف وإضافة سطر توقيع
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // إضافة صورة تجريبية مع سطر توقيع
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // إنشاء توقيع رقمي
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // تعيين التوقيع الرقمي وحفظه
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            using (MemoryStream output = new MemoryStream())
            {
                wb.Save(output, SaveFormat.Xlsx);
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


