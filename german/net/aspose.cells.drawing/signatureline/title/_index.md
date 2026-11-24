---
title: "SignatureLine.Title"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine Eigenschaft. Gibt oder setzt den Titel des Unterzeichners"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Ruft den Titel des Sängers ab oder legt ihn fest.

```csharp
public string Title { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Signaturzeile und setze ihren Titel
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // Füge die Signaturzeile den Formen des Arbeitsblatts mit Positionsparametern hinzu
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Gib den Titel aus, um zu demonstrieren, dass die Eigenschaft gesetzt wurde
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


