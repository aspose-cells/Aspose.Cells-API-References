---
title: "Cell.IsArrayHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, dass die Formel der Zelle eine Array‑Formel ist und dass sie die erste Zelle des Arrays ist."
type: docs
url: /de/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Gibt an, dass die Formel der Zelle eine Array‑Formel ist und dass sie die erste Zelle des Arrays ist.

```csharp
public bool IsArrayHeader { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Array-Formel im Bereich B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // Überprüfe und gib die Eigenschaft IsArrayHeader aus
            // Hinweis: IsArrayHeader ist schreibgeschützt und wird automatisch für Array-Formel‑Kopfzeilen gesetzt
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


