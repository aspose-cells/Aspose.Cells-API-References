---
title: "Enum SignatureType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.SignatureType enum. Anger signaturtypen"
type: docs
url: /sv/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

Anger signaturtypen.

```csharp
public enum SignatureType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Standardvärdet, det motsvarande ProviderId‑värdet är fastställt till {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | Det motsvarande ProviderId‑värdet är vanligtvis {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | Det motsvarande ProviderId‑värdet måste vanligtvis anges av användaren. Det bör hämtas från dokumentationen som levereras med leverantören. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till signaturlinjer med olika typer
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Spara arbetsboken med signaturkonfigurationer
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


