---
title: "Worksheet.Zoom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen."
type: docs
url: /de/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen.

```csharp
public int Zoom { get; set; }
```

### Hinweise

Bitte legen Sie zuerst den Ansichtstyp fest.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie den Zoomfaktor auf 120 %.
            worksheet.Zoom = 120;
            
            // Aktuellen Zoomfaktor anzeigen
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


