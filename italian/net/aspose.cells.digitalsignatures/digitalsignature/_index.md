---
title: "Classe DigitalSignature"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DigitalSignatures.DigitalSignature. Firma nel file"
type: docs
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
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Costruttore di digitalSignature. Utilizza l'implementazione .Net. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Costruttore di digitalSignature. Utilizza l'implementazione Bouncy Castle. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Oggetto certificato utilizzato per firmare il documento. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | Lo scopo della firma. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty (tutti zero) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Specifica un'immagine per la firma digitale. Il valore predefinito è null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Specifica l'ID classe del provider di firma. Il valore predefinito è Empty (tutti zero) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | Il tempo in cui il documento è stato firmato. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | Tipo XAdES. Il valore predefinito è None (XAdES è disattivato). |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Crea una firma digitale utilizzando il costruttore del certificato
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Imposta proprietà aggiuntive
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Aggiungi la firma alla cartella di lavoro
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Visualizza le informazioni della firma
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Salva la cartella di lavoro firmata
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

### Vedi anche

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


