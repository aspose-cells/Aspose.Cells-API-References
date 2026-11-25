---
title: "Classe SignatureLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.SignatureLine. Rappresenta la linea di firma"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Rappresenta la linea della firma.

```csharp
public class SignatureLine
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SignatureLine](signatureline/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Indica se i commenti possono essere allegati. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Ottiene o imposta l'email del firmatario. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Ottiene o imposta l'identificatore per questa linea di firma. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Ottiene o imposta il testo mostrato all'utente al momento della firma. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Indica se è una linea di firma. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Ottiene o imposta l'ID del provider di firma. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Indica se mostra la data di firma. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Ottiene o imposta il tipo di firma. Default - Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a {0000000000-0000-0000-0000-0000000000}. Stamp - Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente {000CD6A4-0000-0000-C000-000000000046}. Custom - Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. Deve essere ottenuto dalla documentazione fornita con il provider. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Ottiene o imposta il firmatario. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Ottiene o imposta il titolo del cantante. |

### Esempi

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
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di un'immagine
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // Crea l'oggetto riga della firma
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

            // Assegna l'oggetto linea di firma alla proprietà Picture.SignatureLine
            pic.SignatureLine = s;

            // Salva il file Excel
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


