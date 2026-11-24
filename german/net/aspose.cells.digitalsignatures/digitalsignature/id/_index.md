---
title: "DigitalSignature.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature property. Gibt einen GUID an, der mit dem GUID der im Dokumentinhalt gespeicherten Signaturzeile abgeglichen werden kann. Standardwert ist ein leerer GUID mit allen Nullen."
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Gibt eine GUID an, die mit der GUID der Signaturzeile, die im Dokumentinhalt gespeichert ist, abgeglichen werden kann. Standardwert ist Empty (alle Nullen) Guid.

```csharp
public Guid Id { get; set; }
```

### Hinweise

Wenn gesetzt, verknüpft es [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) mit der entsprechenden [`DigitalSignature`](../).

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine digitale Signatur mit einer bestimmten ID
            Guid signatureId = Guid.NewGuid();
            
            // Erstellen Sie eine digitale Signatur
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // Setze die Id der Signatur
            signature.Id = signatureId;

            // Signatur zur Sammlung hinzufügen
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Wende digitale Signatur auf die Arbeitsmappe an
            workbook.SetDigitalSignature(dsCollection);

            // Speichere die Arbeitsmappe
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


