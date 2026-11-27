---
title: "DigitalSignature.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-egenskap. Anger ett GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är ett tomt GUID med enbart nollor."
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är Empty (alla nollor) Guid.

```csharp
public Guid Id { get; set; }
```

### Anmärkningar

När den är inställd associerar den [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) med motsvarande [`DigitalSignature`](../).

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en digital signatur med ett specifikt ID
            Guid signatureId = Guid.NewGuid();
            
            // Skapa en digital signatur
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // Ange signaturens Id
            signature.Id = signatureId;

            // Lägg till signatur i samlingen
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Applicera digital signatur på arbetsboken
            workbook.SetDigitalSignature(dsCollection);

            // Spara arbetsboken
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


