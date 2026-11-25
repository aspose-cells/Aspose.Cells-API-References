---
title: "ScenarioInputCell.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioInputCell. Ottiene e imposta l'indice di colonna della cella di input"
type: docs
url: /it/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Ottiene e imposta l'indice di colonna della cella di input.

```csharp
public int Column { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
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

            // Accedi e dimostra la proprietà Column
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Poiché Column è di sola lettura, dobbiamo rimuovere e riaggiungere per cambiare la colonna
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Verifica la modifica
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Salva la cartella di lavoro
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


