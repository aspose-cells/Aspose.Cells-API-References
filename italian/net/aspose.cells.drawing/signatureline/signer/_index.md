---
title: "SignatureLine.Signer"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SignatureLine. Ottiene o imposta il firmatario"
type: docs
url: /it/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

Ottiene o imposta il firmatario.

```csharp
public string Signer { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una linea di firma e imposta le sue proprietà
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // Aggiungi la linea di firma al foglio di lavoro nella riga 1, colonna 1
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

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


