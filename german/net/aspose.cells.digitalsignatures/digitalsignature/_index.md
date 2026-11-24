---
title: "Klasse DigitalSignature"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DigitalSignatures.DigitalSignature Klasse. Signatur in Datei"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Signatur in Datei.

```csharp
public class DigitalSignature
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Konstruktor von digitalSignature. Verwendet .Net-Implementierung. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Konstruktor von digitalSignature. Verwendet Bouncy‑Castle-Implementierung. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | Der Zweck der Signatur. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Gibt eine GUID an, die mit der GUID der Signaturzeile, die im Dokumentinhalt gespeichert ist, abgeglichen werden kann. Standardwert ist Empty (alle Nullen) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Gibt ein Bild für die digitale Signatur an. Standardwert ist null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Wenn diese digitale Signatur gültig ist und das Dokument nicht manipuliert wurde, ist dieser Wert wahr. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist Empty (alle Nullen) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | Der Zeitpunkt, zu dem das Dokument signiert wurde. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | XAdES-Typ. Standardwert ist None (XAdES ist deaktiviert). |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Erstelle eine digitale Signatur mit dem Zertifikatskonstruktor
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Zusätzliche Eigenschaften festlegen
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Signatur zum Arbeitsbuch hinzufügen
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Signaturinformationen anzeigen
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Das signierte Arbeitsbuch speichern
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

### Siehe auch

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


