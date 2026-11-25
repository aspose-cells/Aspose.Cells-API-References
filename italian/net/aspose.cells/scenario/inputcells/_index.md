---
title: "Scenario.InputCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Scenario. Ottiene le celle di input dello scenario"
type: docs
url: /it/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Ottiene le celle di input dello scenario.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno scenario al foglio di lavoro
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Aggiungi celle di input allo scenario usando la proprietà InputCells
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // Modifica il valore della prima cella di input
            inputCells[0].Value = "150";

            // Salva la cartella di lavoro
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


