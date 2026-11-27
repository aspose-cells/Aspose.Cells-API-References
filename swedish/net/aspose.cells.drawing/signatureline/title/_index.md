---
title: "SignatureLine.Title"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine egenskap. Hämtar eller anger titeln för signatören"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Hämtar eller anger titeln för sångaren.

```csharp
public string Title { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en signaturlinje och ange dess titel
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // Lägg till signaturlinjen i kalkylbladets former med positionsparametrar
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Skriv ut titeln för att demonstrera att egenskapen har satts
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### Se även

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


