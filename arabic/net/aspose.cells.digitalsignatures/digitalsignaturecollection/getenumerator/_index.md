---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DigitalSignatureCollection. احصل على المتكرر لـ DigitalSignatureCollection هذا المتكرر يسمح بالتكرار عبر المجموعة"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

احصل على المُعدِّد لـ DigitalSignatureCollection، هذا المُعدِّد يسمح بالتكرار عبر المجموعة

```csharp
public IEnumerator GetEnumerator()
```

### قيمة الإرجاع

المتكرر للتكرار.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Collections;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // إنشاء مجموعة توقيع رقمي جديدة
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // إنشاء توقيعات رقمية نموذجية مع المعلمات المطلوبة
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // إضافة توقيعات إلى المجموعة
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // احصل على المتكرر
                IEnumerator enumerator = signatures.GetEnumerator();

                Console.WriteLine("Iterating through digital signatures:");
                int count = 0;
                while (enumerator.MoveNext())
                {
                    DigitalSignature current = (DigitalSignature)enumerator.Current;
                    Console.WriteLine($"Signature #{++count} found");
                }

                Console.WriteLine($"Total signatures: {count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


