---
title: "Worksheet.TransitionEvaluation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om alternativet för Lotus-kompatibilitet för Transition Formula Evaluation är aktiverat"
type: docs
url: /sv/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Anger om alternativet Transition Formula Evaluation (Lotus-kompatibilitet) är aktiverat.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange TransitionEvaluation-egenskap
            worksheet.TransitionEvaluation = true;
            
            // Visa egenskapens värde
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


