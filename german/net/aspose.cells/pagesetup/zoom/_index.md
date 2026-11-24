---
title: "PageSetup.Zoom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen."
type: docs
url: /de/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen.

```csharp
public int Zoom { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zoomstufe auf 150 % setzen
            worksheet.PageSetup.Zoom = 150;
            
            // Aktuelle Zoomstufe drucken
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


