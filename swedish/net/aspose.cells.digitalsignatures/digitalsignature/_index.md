---
title: DigitalSignature
second_title: Aspose.Cells för .NET API-referens
description: Signatur i fil.
type: docs
weight: 1390
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Signatur i fil.

```csharp
public class DigitalSignature
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [DigitalSignature](digitalsignature#constructor_1)(X509Certificate2, string, DateTime) | Konstruktör av digitalSignature. Använder .Net-implementering. |
| [DigitalSignature](digitalsignature#constructor)(byte[], string, string, DateTime) | Konstruktör av digitalSignature. Använder Bouncy Castle-implementering. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate) { get; set; } | Certifikatobjekt som användes för att signera dokumentet. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments) { get; set; } | Syftet med signaturen. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id) { get; set; } | Anger en GUID som kan korsreferens med GUID för signaturraden som är lagrad i dokumentinnehållet. Standardvärdet är Empty (alla nollor) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image) { get; set; } | Anger en bild för den digitala signaturen. Standardvärdet är null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid) { get; } | Om denna digitala signatur är giltig och dokumentet inte har manipulerats, kommer detta värde att vara sant. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid) { get; set; } | Anger klass-ID för signaturleverantören. Standardvärdet är Empty (alla nollor) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime) { get; set; } | Tiden då dokumentet signerades. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text) { get; set; } | Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype) { get; set; } | XAdES-typ. Standardvärdet är Inget (XAdES är avstängt). |

### Se även

* namnutrymme [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->