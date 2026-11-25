---
title: "ScenarioInputCell.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ScenarioInputCell proprietà. Ottiene e imposta il valore della cella di input"
type: docs
url: /it/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Ottiene e imposta il valore della cella di input.

```csharp
public string Value { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno scenario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Aggiungi celle di input con valori
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Accedi e modifica i valori
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Salva la cartella di lavoro
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


