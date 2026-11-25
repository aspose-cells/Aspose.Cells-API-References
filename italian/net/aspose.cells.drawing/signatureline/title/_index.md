---
title: "SignatureLine.Title"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SignatureLine property. Ottiene o imposta il titolo del firmatario"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Ottiene o imposta il titolo del cantante.

```csharp
public string Title { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una linea di firma e imposta il suo titolo
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // Aggiungi la linea di firma alle forme del foglio di lavoro con i parametri di posizione
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Stampa il titolo per dimostrare che la proprietà è stata impostata
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### Vedi anche

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


