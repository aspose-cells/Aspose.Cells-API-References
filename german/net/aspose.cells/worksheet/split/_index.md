---
title: "Worksheet.Split"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Teilt das Fenster"
type: docs
url: /de/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Teilt das Fenster.

```csharp
public void Split()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen, um die Aufteilung zu demonstrieren
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Arbeitsblatt teilen (keine Parameter erforderlich)
            worksheet.Split();
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


