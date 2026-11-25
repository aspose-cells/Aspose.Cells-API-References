---
title: "SignatureLine.IsLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SignatureLine. Indica se è una linea di firma"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Indica se è una linea di firma.

```csharp
public bool IsLine { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIsLineDemo
    {
        public static void Run()
        {
            // Crea un'istanza di linea di firma
            SignatureLine signature = new SignatureLine();
            
            // Imposta IsLine su true
            signature.IsLine = true;
            
            // Verifica e dimostra l'uso di IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // Attiva/disattiva lo stato di IsLine
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### Vedi anche

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


