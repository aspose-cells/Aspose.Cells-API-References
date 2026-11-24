---
title: "SignatureLine.Email"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine Eigenschaft. Gibt oder setzt die E-Mail des Unterzeichners"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Liest oder setzt die E‑Mail des Unterzeichners.

```csharp
public string Email { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Signaturzeile
            SignatureLine signatureLine = new SignatureLine();
            
            // Setze Signaturzeilen-Eigenschaften einschließlich Email
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // Zeige die Email-Eigenschaft an
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


