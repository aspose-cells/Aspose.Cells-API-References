---
title: "SignatureLine.Email"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine egenskap. Hämtar eller anger e-post för signatören"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Hämtar eller anger e‑postadressen för undertecknaren.

```csharp
public string Email { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Skapa en ny signaturlinje
            SignatureLine signatureLine = new SignatureLine();
            
            // Ställ in egenskaper för signaturlinje inklusive e‑post
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // Visa e‑postegenskapen
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### Se även

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


