---
title: "Klass SignatureLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.SignatureLine klass. Representerar signaturlinjen"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Representerar signaturlinjen.

```csharp
public class SignatureLine
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SignatureLine](signatureline/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Indikerar om kommentarer kan bifogas. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Hämtar eller anger e‑postadressen för undertecknaren. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Hämtar eller anger identifieraren för denna signaturlinje. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Hämtar eller anger texten som visas för användaren vid signering. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Indikerar om det är en signaturlinje. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Hämtar eller anger id för signaturleverantör. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Indikerar om signeringsdatum ska visas. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Hämtar eller anger signaturtypen. Default - När standardvärdet är angivet är motsvarande ProviderId‑värde fixerat till {0000000000-0000-0000-0000-0000000000}. Stamp - När värdet är Stamp är motsvarande ProviderId‑värde vanligtvis {000CD6A4-0000-0000-C000-000000000046}. Custom - När värdet är Custom måste motsvarande ProviderId‑värde vanligtvis anges av användaren. Det bör hämtas från dokumentationen som medföljer leverantören. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Hämtar eller anger undertecknaren. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Hämtar eller anger titeln för sångaren. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till en bild
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // Skapa signaturlinjeobjekt
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // Tilldela signaturlinjeobjektet till egenskapen Picture.SignatureLine
            pic.SignatureLine = s;

            // Spara Excel-filen
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


