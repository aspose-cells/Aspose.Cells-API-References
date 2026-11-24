---
title: "Worksheet.TransitionEntry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob die Lotus‑Kompatibilitätsoption für den Transition Formula Entry aktiviert ist"
type: docs
url: /de/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Gibt an, ob die Option Transition Formula Entry (Lotus‑Kompatibilität) aktiviert ist.

```csharp
public bool TransitionEntry { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Legen Sie die TransitionEntry‑Eigenschaft fest
            worksheet.TransitionEntry = true;
            
            // Den TransitionEntry-Wert anzeigen
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Laden Sie die gespeicherte Arbeitsmappe, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Den geladenen TransitionEntry-Wert anzeigen
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


