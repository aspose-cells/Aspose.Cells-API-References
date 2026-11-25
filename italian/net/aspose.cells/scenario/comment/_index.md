---
title: "Scenario.Comment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Scenario. Ottiene e imposta il commento dello scenario"
type: docs
url: /it/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Ottiene e imposta il commento dello scenario.

```csharp
public string Comment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una raccolta di scenari
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Aggiungi uno scenario
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Imposta le proprietà dello scenario
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Aggiungi celle di input allo scenario usando riferimenti di cella e valori
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Visualizza il commento dello scenario
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Salva la cartella di lavoro
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


