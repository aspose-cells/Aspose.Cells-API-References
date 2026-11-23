---
title: "ScenarioCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScenarioCollection. Obtient l'objet Scenario par l'index"
type: docs
url: /fr/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Obtient l'objet [`Scenario`](../../scenario/) par l'index.

```csharp
public Scenario this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index spécifique dans la liste. |

### Exemples

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

            // Démontrer l'utilisation de la propriété Item
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


