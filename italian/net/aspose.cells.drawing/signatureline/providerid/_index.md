---
title: "SignatureLine.ProviderId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SignatureLine property. Ottiene o imposta l'ID del provider della firma"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Ottiene o imposta l'ID del provider di firma.

```csharp
public Guid ProviderId { get; set; }
```

### Osservazioni

Di solito è il CLSID del componente aggiuntivo COM del provider.

### Esempi

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Crea una nuova linea di firma
            SignatureLine signatureLine = new SignatureLine();
            
            // Imposta le proprietà della linea di firma
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Imposta l'ID del provider (GUID di esempio - dovrebbe essere sostituito con il GUID reale del provider)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // Imposta il tipo di firma (questo dovrebbe corrispondere all'ID del provider)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Stampa l'ID del provider per dimostrare l'uso
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### Vedi anche

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


