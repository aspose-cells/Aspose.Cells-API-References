---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignatureCollection-konstruktör. Konstruktören för DigitalSignatureCollection"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

Konstruktorn för DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### Exempel

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
            // Initiera en ny DigitalSignatureCollection
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // Läs in certifikat och skapa digital signatur
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // Lägg till signatur i samlingen
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### Se även

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


