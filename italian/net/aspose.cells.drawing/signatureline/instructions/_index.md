---
title: "SignatureLine.Instructions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SignatureLine property. Ottiene o imposta il testo mostrato all'utente al momento della firma"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

Ottiene o imposta il testo mostrato all'utente al momento della firma.

```csharp
public string Instructions { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un oggetto linea di firma
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // Aggiungi la linea di firma al foglio di lavoro nella posizione (1,1)
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

            // Salva la cartella di lavoro
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


