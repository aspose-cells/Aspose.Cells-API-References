---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DigitalSignatureCollection. Il costruttore di DigitalSignatureCollection"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

Il costruttore di DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### Esempi

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
            // Inizializza una nuova DigitalSignatureCollection
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // Carica il certificato e crea la firma digitale
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // Aggiungi la firma alla raccolta
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### Vedi anche

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


