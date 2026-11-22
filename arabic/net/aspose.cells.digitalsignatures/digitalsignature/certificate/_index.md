---
title: "DigitalSignature.Certificate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. كائن الشهادة الذي تم استخدامه لتوقيع المستند"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

كائن الشهادة الذي تم استخدامه لتوقيع المستند.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyCertificateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء شهادة (في السيناريو الحقيقي، ستحمل شهادة فعلية)
            // هذا فقط للعرض - لن يكون صالحًا للتوقيع الفعلي
            X509Certificate2 certificate = new X509Certificate2();
            
            // إنشاء توقيع رقمي باستخدام الشهادة
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // عرض معلومات الشهادة الحالية
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // إنشاء مجموعة وإضافة التوقيع إليها
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // إضافة التوقيعات إلى دفتر العمل
            workbook.AddDigitalSignature(signatureCollection);
            
            // إنشاء شهادة جديدة (محاكاة)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // تغيير خاصية الشهادة
            signature.Certificate = newCertificate;
            
            // عرض معلومات الشهادة الجديدة
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // حفظ المصنف مع التوقيع الرقمي
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


