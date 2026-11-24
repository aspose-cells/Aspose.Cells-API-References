---
title: "SignatureLine.Signer"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine-Eigenschaft. Gibt den Unterzeichner zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

Ruft den Unterzeichner ab oder legt ihn fest.

```csharp
public string Signer { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Signaturzeile und setze ihre Eigenschaften
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // Füge die Signaturzeile dem Arbeitsblatt in Zeile 1, Spalte 1 hinzu
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Speichere die Arbeitsmappe
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


