---
title: "Worksheet.Scenarios"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la raccolta di Scenario"
type: docs
url: /it/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

Ottiene la raccolta di [`Scenario`](../../scenario/).

```csharp
public ScenarioCollection Scenarios { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Aggiungi scenari
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // Cancella gli scenari e salva di nuovo
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


