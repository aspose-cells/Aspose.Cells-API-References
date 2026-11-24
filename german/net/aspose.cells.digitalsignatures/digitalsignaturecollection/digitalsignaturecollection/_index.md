---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignatureCollection Konstruktor. Der Konstruktor von DigitalSignatureCollection"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

Der Konstruktor von DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### Beispiele

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
            // Initialisiere eine neue DigitalSignatureCollection
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // Lade das Zertifikat und erstelle eine digitale Signatur
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // Signatur zur Sammlung hinzufügen
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### Siehe auch

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


