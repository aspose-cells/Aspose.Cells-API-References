---
title: "ScenarioInputCell.IsDeleted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioInputCell. Indica se la cella di input è eliminata"
type: docs
url: /it/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Indica se la cella di input è eliminata.

```csharp
public bool IsDeleted { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno scenario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Aggiungi celle di input
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Accedi e visualizza le celle di input
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // Elimina la prima cella di input
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Salva la cartella di lavoro
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


