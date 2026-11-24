---
title: "SignatureLine.Instructions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine Eigenschaft. Gibt oder setzt den Text, der dem Benutzer zur Signaturzeit angezeigt wird"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

Liest oder setzt den Text, der dem Benutzer zur Signaturzeit angezeigt wird.

```csharp
public string Instructions { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Signaturzeilen-Objekt
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // Füge die Signaturzeile dem Arbeitsblatt an Position (1,1) hinzu
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

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


