---
title: "Enum SignatureType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.SignatureType. Specifica il tipo di firma"
type: docs
url: /it/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

Specifica il tipo di firma.

```csharp
public enum SignatureType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Il valore predefinito, il valore ProviderId corrispondente è fissato a {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | Il valore ProviderId corrispondente è solitamente {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | Il valore ProviderId corrispondente di solito deve essere impostato dall'utente. Deve essere ottenuto dalla documentazione fornita con il provider. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi linee di firma con tipi diversi
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Salva la cartella di lavoro con le configurazioni della firma
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


