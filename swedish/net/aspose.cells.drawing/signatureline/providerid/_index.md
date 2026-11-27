---
title: "SignatureLine.ProviderId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine egenskap. Hämtar eller anger id för signaturleverantören"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Hämtar eller anger id för signaturleverantör.

```csharp
public Guid ProviderId { get; set; }
```

### Anmärkningar

Det är vanligtvis CLSID för leverantörens COM-tillägg.

### Exempel

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Skapa en ny signaturlinje
            SignatureLine signatureLine = new SignatureLine();
            
            // Ange egenskaper för signaturlinje
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Ange leverantörs-ID (exempel GUID - bör ersättas med faktiskt leverantörs-GUID)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // Ange signaturtyp (detta bör matcha leverantörs-ID)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Skriv ut leverantörs-ID för att demonstrera användning
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### Se även

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


