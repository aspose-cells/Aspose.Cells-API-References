---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignatureCollection yapıcı. DigitalSignatureCollection'ın yapıcısı"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

DigitalSignatureCollection sınıfının yapıcısı.

```csharp
public DigitalSignatureCollection()
```

### Örnekler

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
            // Yeni bir DigitalSignatureCollection başlatın
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // Sertifikayı yükleyin ve dijital imza oluşturun
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // İmzayı koleksiyona ekleyin
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


