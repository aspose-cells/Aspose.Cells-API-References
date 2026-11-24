---
title: "Worksheet.IsPageBreakPreview"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob das angegebene Arbeitsblatt in der Normalansicht oder in der Seitenumbruchvorschau angezeigt wird"
type: docs
url: /de/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Gibt an, ob das angegebene Arbeitsblatt in der Normalansicht oder in der Seitenumbruchvorschau angezeigt wird.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzt das Arbeitsblatt in den Seitenumbruchvorschau-Modus
            worksheet.IsPageBreakPreview = true;
            
            // Zoom auf 100 % für die Demonstration einstellen
            worksheet.Zoom = 100;
            
            // Gibt die aktuellen Einstellungen aus
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


