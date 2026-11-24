---
title: "SignatureLine.IsLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine-Eigenschaft. Gibt an, ob es sich um eine Signaturzeile handelt"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Gibt an, ob es sich um eine Signaturzeile handelt.

```csharp
public bool IsLine { get; set; }
```

### Beispiele

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
            // Erstelle eine Instanz einer Signaturzeile
            SignatureLine signature = new SignatureLine();
            
            // Setze IsLine auf true
            signature.IsLine = true;
            
            // Überprüfe und demonstriere die Verwendung von IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // Schalte den IsLine-Status um
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


