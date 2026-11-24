---
title: "Cells.IsDefaultRowHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt an, ob die Zeile standardmäßig ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Gibt an, ob die Zeile standardmäßig ausgeblendet ist.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Standardmäßig ausgeblendete Zeilen-Eigenschaft festlegen
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // Zeige den aktuellen Wert von IsDefaultRowHidden an
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


