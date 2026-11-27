---
title: "SignatureLine.Signer"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine‑egenskap. Hämtar eller anger undertecknaren"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

Hämtar eller anger undertecknaren.

```csharp
public string Signer { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en signaturlinje och ställ in dess egenskaper
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // Lägg till signaturlinjen i kalkylbladet på rad 1, kolumn 1
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

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


