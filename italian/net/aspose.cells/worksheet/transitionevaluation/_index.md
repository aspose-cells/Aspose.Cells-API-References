---
title: "Worksheet.TransitionEvaluation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet property. Indica se l'opzione di compatibilità Lotus per la valutazione della formula di transizione è abilitata"
type: docs
url: /it/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Indica se l'opzione Transition Formula Evaluation (compatibilità Lotus) è abilitata.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la proprietà TransitionEvaluation
            worksheet.TransitionEvaluation = true;
            
            // Visualizza il valore della proprietà
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


