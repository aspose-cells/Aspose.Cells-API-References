---
title: "ScenarioCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioCollection egenskap. Hämtar Scenario-objektet efter indexet"
type: docs
url: /sv/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Hämtar [`Scenario`](../../scenario/) objektet efter indexet.

```csharp
public Scenario this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det specifika indexet i listan. |

### Exempel

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

            // Demonstrera användning av Item-egenskapen
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


