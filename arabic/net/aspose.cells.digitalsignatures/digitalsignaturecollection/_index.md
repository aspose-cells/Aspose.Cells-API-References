---
title: "فئة DigitalSignatureCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.DigitalSignatures.DigitalSignatureCollection. توفر مجموعة من التوقيعات الرقمية المرفقة بمستند"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

يوفر مجموعة من التوقيعات الرقمية المرفقة بمستند.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | المُنشئ الخاص بـ DigitalSignatureCollection. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | أضف توقيعًا واحدًا إلى DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | احصل على المُعدِّد لـ DigitalSignatureCollection، هذا المُعدِّد يسمح بالتكرار عبر المجموعة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionDemo
    {
        public static void DigitalSignatureCollectionExample()
        {
            // حمّل مصنفًا من ملف مصدر موقع
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // تحقق مما إذا كان المصنف موقعًا رقميًا
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // احصل على مجموعة التوقيع الرقمي من المصنف
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // تجول عبر التوقيعات الرقمية في المجموعة
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // أنشئ توقيعًا رقميًا جديدًا
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // أضف التوقيع الرقمي الجديد إلى المجموعة
                existingDsc.Add(newSignature);
            }     
            

            // احفظ المصنف مع التوقيع الرقمي الجديد
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


