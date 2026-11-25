---
title: "SignatureLine.Email"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SignatureLine property. Ottiene o imposta l'email del firmatario"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Ottiene o imposta l'email del firmatario.

```csharp
public string Email { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Crea una nuova linea di firma
            SignatureLine signatureLine = new SignatureLine();
            
            // Imposta le proprietà della linea di firma includendo l'e-mail
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // Visualizza la proprietà e-mail
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### Vedi anche

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


