---
title: "DigitalSignatureCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignatureCollection yöntemi. DigitalSignatureCollection'a bir imza ekleyin"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/
---
## DigitalSignatureCollection.Add method

DigitalSignatureCollection'a bir imza ekleyin.

```csharp
public void Add(DigitalSignature digitalSignature)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| digitalSignature | DigitalSignature | Koleksiyondaki dijital imza. |

### Örnekler

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

### Ayrıca Bakınız

* class [DigitalSignature](../../digitalsignature/)
* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


