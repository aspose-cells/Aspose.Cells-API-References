---
title: "DigitalSignatureCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DigitalSignatureCollection. أضف توقيعًا واحدًا إلى DigitalSignatureCollection"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/
---
## DigitalSignatureCollection.Add method

أضف توقيعًا واحدًا إلى DigitalSignatureCollection.

```csharp
public void Add(DigitalSignature digitalSignature)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignature | DigitalSignature | التوقيع الرقمي في المجموعة. |

### أمثلة

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureCollectionMethodAddWithDigitalSignatureDemo
    {
        public static void Run()
        {
            string password = "1234567890";
            string sourcePath = "example.xlsx";
            string destPath = "signed_example.xlsx";

            Workbook workbook = new Workbook(sourcePath);

            X509Certificate2 certificate = new X509Certificate2("test_dsa_sha1_1024.pfx", password);

            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            DigitalSignature signature = new DigitalSignature(certificate, "Test signing", DateTime.Now);
            
            dsCollection.Add(signature);
            workbook.SetDigitalSignature(dsCollection);
            
            workbook.Save(destPath);
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../../digitalsignature/)
* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


