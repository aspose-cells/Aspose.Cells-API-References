---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor DigitalSignatureCollection. El constructor de DigitalSignatureCollection"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

El constructor de DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### Ejemplos

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
            // Inicialice una nueva DigitalSignatureCollection
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // Cargue el certificado y cree una firma digital
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // Agregar firma a la colección
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### Ver también

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


