---
title: "SignatureLine.SignatureLineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SignatureLine. Ottiene o imposta il tipo di firma. Default  Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a 00000000000000000000000000000000. Stamp  Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente 000CD6A400000000C000000000000046. Custom  Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. dovrebbe essere ottenuto dalla documentazione fornita con il provider"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

Ottiene o imposta il tipo di firma. Default - Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a {0000000000-0000-0000-0000-0000000000}. Stamp - Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente {000CD6A4-0000-0000-C000-000000000046}. Custom - Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. Deve essere ottenuto dalla documentazione fornita con il provider.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una linea di firma
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Visualizza il SignatureLineType corrente
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // Imposta SignatureLineType su Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // Aggiungi la linea di firma al foglio di lavoro aggiungendola alle forme
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // Cambia SignatureLineType in Custom con ProviderId personalizzato
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Salva la cartella di lavoro
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


