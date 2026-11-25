---
title: "ScenarioInputCell.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioInputCell. Ottiene e imposta l'indirizzo della cella di input"
type: docs
url: /it/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Ottiene e imposta l'indirizzo della cella di input.

```csharp
public string Name { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno scenario
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Ottieni lo scenario
            Scenario scenario = scenarios[scenarioIndex];

            // Aggiungi le celle di input allo scenario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Ottieni le celle di input
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Dimostra l'uso della proprietà Name
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // Verifica che i nomi corrispondano ai valori attesi
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


