---
title: "Cells.StandardHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt in Punkten."
type: docs
url: /de/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Liest oder legt die Standardzeilenhöhe in diesem Arbeitsblatt in Punkten fest.

```csharp
public double StandardHeight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Standardhöhe abrufen und anzeigen
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Eine neue Standardhöhe festlegen
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Speichere die Arbeitsmappe
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


