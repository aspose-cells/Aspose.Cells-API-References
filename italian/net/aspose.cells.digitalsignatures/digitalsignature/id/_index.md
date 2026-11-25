---
title: "DigitalSignature.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Specifica un GUID che può essere correlato al GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty tutti zero Guid"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty (tutti zero) Guid.

```csharp
public Guid Id { get; set; }
```

### Osservazioni

Quando impostato, associa [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) con la corrispondente [`DigitalSignature`](../).

### Esempi

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una firma digitale con un ID specifico
            Guid signatureId = Guid.NewGuid();
            
            // Crea una firma digitale
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // Imposta l'ID della firma
            signature.Id = signatureId;

            // Aggiungi la firma alla raccolta
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Applica la firma digitale alla cartella di lavoro
            workbook.SetDigitalSignature(dsCollection);

            // Salva la cartella di lavoro
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


