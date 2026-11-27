---
title: "Klass DigitalSignature"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DigitalSignatures.DigitalSignature-klass. Signatur i filen"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Signatur i filen.

```csharp
public class DigitalSignature
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Konstruktor för digitalSignature. Använder .Net-implementation. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Konstruktor för digitalSignature. Använder Bouncy Castle-implementation. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Certifikatobjekt som användes för att signera dokumentet. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | Syftet med signaturen. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är Empty (alla nollor) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Anger en bild för den digitala signaturen. Standardvärdet är null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Om denna digitala signatur är giltig och dokumentet inte har manipulerats, kommer detta värde att vara true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Anger klass-ID för signaturleverantören. Standardvärdet är Empty (alla nollor) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | Tidpunkten då dokumentet signerades. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | XAdES-typ. Standardvärdet är None (XAdES är avstängt). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturesClassDigitalSignatureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Skapa en digital signatur med certifikatkonstruktorn
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Ange ytterligare egenskaper
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Lägg till signatur i arbetsboken
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Visa signaturinformation
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Spara den signerade arbetsboken
                workbook.Save("DigitalSignatureDemo.xlsx");
                Console.WriteLine("Workbook signed and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DigitalSignature: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


