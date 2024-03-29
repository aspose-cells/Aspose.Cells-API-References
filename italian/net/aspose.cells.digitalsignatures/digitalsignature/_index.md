---
title: DigitalSignature
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Firma nel file.
type: docs
weight: 1390
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Firma nel file.

```csharp
public class DigitalSignature
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DigitalSignature](digitalsignature#constructor_1)(X509Certificate2, string, DateTime) | Costruttore di firma digitale. Utilizza l'implementazione .Net. |
| [DigitalSignature](digitalsignature#constructor)(byte[], string, string, DateTime) | Costruttore di firma digitale. Utilizza l'implementazione del castello gonfiabile. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate) { get; set; } | Oggetto certificato utilizzato per firmare il documento. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments) { get; set; } | Lo scopo della firma. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id) { get; set; } | Specifica un GUID che può essere incrociato con il GUID della riga della firma memorizzata nel contenuto del documento. Il valore predefinito è Vuoto (tutti zeri) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image) { get; set; } | Specifica un'immagine per la firma digitale. Il valore predefinito è null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid) { get; } | Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid) { get; set; } | Specifica l'ID classe del provider di firma. Il valore predefinito è Vuoto (tutti zeri) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime) { get; set; } | L'ora in cui il documento è stato firmato. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text) { get; set; } | Specifica il testo della firma effettiva nella firma digitale. Il valore predefinito è Vuoto. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype) { get; set; } | Tipo XAdES. Il valore predefinito è Nessuno(XAdES è disattivato). |

### Guarda anche

* spazio dei nomi [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
