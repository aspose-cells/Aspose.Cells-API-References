---
title: "SignatureLine.ProviderId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine Eigenschaft. Gibt oder setzt die ID des Signaturproviders"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Liest oder setzt die ID des Signaturanbieters.

```csharp
public Guid ProviderId { get; set; }
```

### Hinweise

Es ist typischerweise die CLSID des Provider-COM-Add-Ins.

### Beispiele

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Signaturzeile
            SignatureLine signatureLine = new SignatureLine();
            
            // Setze Eigenschaften der Signaturzeile
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Setze Provider-ID (Beispiel-GUID - sollte durch die tatsächliche Provider-GUID ersetzt werden)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // Setze Signaturtyp (dies sollte mit der Provider-ID übereinstimmen)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Gib die Provider-ID aus, um die Verwendung zu demonstrieren
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


