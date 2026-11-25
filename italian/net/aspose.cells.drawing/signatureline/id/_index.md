---
title: "SignatureLine.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SignatureLine property. Ottiene o imposta l'identificatore per questa linea di firma"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Ottiene o imposta l'identificatore per questa linea di firma.

```csharp
public Guid Id { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un oggetto linea di firma
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // Aggiungi la linea di firma al foglio di lavoro nella posizione (1,1)
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Visualizza l'ID della linea di firma
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### Vedi anche

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


