---
title: "ScenarioCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioCollection-Eigenschaft. Gibt das Scenario-Objekt anhand des Index zurück"
type: docs
url: /de/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Gibt das [`Scenario`](../../scenario/)‑Objekt anhand des Index zurück.

```csharp
public Scenario this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der spezifische Index in der Liste. |

### Beispiele

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

            // Demonstriere die Verwendung der Item-Eigenschaft
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


