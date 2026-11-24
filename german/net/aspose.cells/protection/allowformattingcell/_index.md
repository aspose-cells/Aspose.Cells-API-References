---
title: "Protection.AllowFormattingCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection property. Gibt an, ob die Formatierung von Zellen in einem geschützten Arbeitsblatt erlaubt ist"
type: docs
url: /de/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Stellt dar, ob das Formatieren von Zellen in einem geschützten Arbeitsblatt erlaubt ist.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblattschutz aktivieren
            Protection protection = worksheet.Protection;
            
            // Setzen Sie verschiedene Schutz-Eigenschaften mithilfe eines Flags
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Überprüfen Sie die Einstellung
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


