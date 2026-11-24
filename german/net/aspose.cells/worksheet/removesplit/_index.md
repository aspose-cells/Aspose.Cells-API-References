---
title: "Worksheet.RemoveSplit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Entfernt das geteilte Fenster"
type: docs
url: /de/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Entfernt geteiltes Fenster.

```csharp
public void RemoveSplit()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Worksheet teilen
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Entferne die Teilung
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


