---
title: "SignatureLine.SignatureLineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SignatureLine‑egenskap. Hämtar eller anger signaturtypen. Default  När standardvärdet är angivet är motsvarande ProviderId‑värde fixerat till 00000000000000000000000000000000. Stamp  När värdet är Stamp är motsvarande ProviderId‑värde vanligtvis 000CD6A400000000C000000000000046. Custom  När värdet är Custom måste motsvarande ProviderId‑värde vanligtvis anges av användaren. det bör hämtas från dokumentationen som medföljer leverantören"
type: docs
url: /sv/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

Hämtar eller anger signaturtypen. Default - När standardvärdet är angivet är motsvarande ProviderId‑värde fixerat till {0000000000-0000-0000-0000-0000000000}. Stamp - När värdet är Stamp är motsvarande ProviderId‑värde vanligtvis {000CD6A4-0000-0000-C000-000000000046}. Custom - När värdet är Custom måste motsvarande ProviderId‑värde vanligtvis anges av användaren. Det bör hämtas från dokumentationen som medföljer leverantören.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en signaturlinje
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Visa aktuell SignatureLineType
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // Ställ in SignatureLineType till Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // Lägg till signaturlinjen i kalkylbladet genom att lägga till den i former
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // Ändra SignatureLineType till Custom med anpassad ProviderId
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Spara arbetsboken
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


