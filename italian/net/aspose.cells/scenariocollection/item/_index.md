---
title: "ScenarioCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioCollection. Ottiene l'oggetto Scenario per indice"
type: docs
url: /it/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Ottiene l'oggetto [`Scenario`](../../scenario/) per indice.

```csharp
public Scenario this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice specifico nell'elenco. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            scenario.InputCells.Add(0, 0, "100");
            scenario.InputCells.Add(1, 1, "200");

            // Dimostra l'uso della proprietà Item
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


