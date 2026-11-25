---
title: "Classe ScenarioInputCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ScenarioInputCell. Rappresenta la cella di input per lo scenario"
type: docs
url: /it/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Rappresenta la cella di input per lo scenario.

```csharp
public class ScenarioInputCell
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Ottiene e imposta l'indice di colonna della cella di input. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Indica se la cella di input è eliminata. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Ottiene e imposta l'indirizzo della cella di input. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Ottiene e imposta l'indice di riga della cella di input. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Ottiene e imposta il valore della cella di input. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno scenario al foglio di lavoro
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Aggiungi le celle di input allo scenario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Accesso alle celle di input
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Visualizzazione delle proprietà delle celle di input
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Modifica il valore della prima cella di input
            inputCell1.Value = "150";

            // Salva la cartella di lavoro
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


