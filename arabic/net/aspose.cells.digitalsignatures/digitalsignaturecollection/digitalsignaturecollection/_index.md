---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DigitalSignatureCollection. منشئ DigitalSignatureCollection"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

المُنشئ الخاص بـ DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### أمثلة

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureCollectionMethodCtorDemo
    {
        public static void Run()
        {
            // تهيئة DigitalSignatureCollection جديد
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // تحميل الشهادة وإنشاء توقيع رقمي
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // إضافة توقيع إلى المجموعة
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


