---
title: "SignatureLine.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine Eigenschaft. Gibt oder setzt den Bezeichner für diese Signaturzeile"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Liest oder setzt den Bezeichner für diese Signaturzeile.

```csharp
public Guid Id { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Signaturzeilen-Objekt
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // Füge die Signaturzeile dem Arbeitsblatt an Position (1,1) hinzu
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Zeige die ID der Signaturzeile an
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


