---
title: "SignatureLine.Instructions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine egenskap. Hämtar eller anger den text som visas för användaren vid signeringstidpunkten"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

Hämtar eller anger texten som visas för användaren vid signering.

```csharp
public string Instructions { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett signaturlinjeobjekt
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // Lägg till signaturlinjen i kalkylbladet på position (1,1)
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

            // Spara arbetsboken
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Se även

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


