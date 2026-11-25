---
title: "ScenarioInputCell.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioInputCell. Ottiene e imposta l'indice di riga della cella di input"
type: docs
url: /it/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Ottiene e imposta l'indice di riga della cella di input.

```csharp
public int Row { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno scenario al foglio di lavoro
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Aggiungi le celle di input allo scenario
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Accedi e dimostra la proprietà Row
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Aggiungi una nuova cella alla riga 2 invece di provare a modificare quella esistente
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Salva la cartella di lavoro
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


