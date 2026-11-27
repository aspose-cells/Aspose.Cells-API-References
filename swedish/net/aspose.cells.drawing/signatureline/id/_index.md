---
title: "SignatureLine.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine egenskap. Hämtar eller anger identifierare för denna signaturlinje"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Hämtar eller anger identifieraren för denna signaturlinje.

```csharp
public Guid Id { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett signaturlinjeobjekt
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // Lägg till signaturlinjen i kalkylbladet på position (1,1)
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Visa ID för signaturlinjen
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### Se även

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


