---
title: "Worksheet.TransitionEvaluation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob die Lotus‑Kompatibilitätsoption für die Übergangsformelauswertung aktiviert ist"
type: docs
url: /de/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Gibt an, ob die Option Transition Formula Evaluation (Lotus‑Kompatibilität) aktiviert ist.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // TransitionEvaluation‑Eigenschaft festlegen
            worksheet.TransitionEvaluation = true;
            
            // Den Eigenschaftswert anzeigen
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Laden Sie die gespeicherte Arbeitsmappe, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


