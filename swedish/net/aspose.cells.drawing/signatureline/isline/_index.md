---
title: "SignatureLine.IsLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine‑egenskap. Anger om det är en signaturlinje"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Indikerar om det är en signaturlinje.

```csharp
public bool IsLine { get; set; }
```

### Exempel

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
            // Skapa en instans av signaturlinje
            SignatureLine signature = new SignatureLine();
            
            // Ställ in IsLine till true
            signature.IsLine = true;
            
            // Kontrollera och demonstrera användning av IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // Växla IsLine‑tillstånd
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### Se även

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


