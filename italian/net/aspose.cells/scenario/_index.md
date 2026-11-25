---
title: "Classe Scenario"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Scenario. Rappresenta uno scenario individuale"
type: docs
url: /it/net/aspose.cells/scenario/
---
## Scenario class

Rappresenta uno scenario individuale.

```csharp
public class Scenario
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Ottiene e imposta il commento dello scenario. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Ottiene le celle di input dello scenario. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Indica se lo scenario è nascosto. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Indica se lo scenario è bloccato per la modifica quando il foglio è protetto. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Ottiene e imposta il nome dello scenario. |
| [User](../../aspose.cells/scenario/user/) { get; } | Ottiene il nome dell'utente che ha modificato per ultimo lo scenario. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla raccolta di scenari del foglio di lavoro
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Aggiungi un nuovo scenario alla collezione
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Impostazione delle proprietà dello scenario
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Accesso alle proprietà di sola lettura
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Salva la cartella di lavoro
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


