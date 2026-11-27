---
title: "ScenarioInputCellCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioInputCellCollection metod. Lägger till en inmatningscell"
type: docs
url: /sv/net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Lägger till en inmatningscell.

```csharp
public int Add(int row, int column, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet för inmatningscellen. |
| column | Int32 | Kolumnindexet för inmatningscellen. |
| värde | String | Värdet på inmatningscellen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            Console.WriteLine($"Count: {inputCells.Count}");
            Console.WriteLine($"Cell 1: Row={inputCells[0].Row}, Column={inputCells[0].Column}, Value={inputCells[0].Value}");
            Console.WriteLine($"Cell 2: Row={inputCells[1].Row}, Column={inputCells[1].Column}, Value={inputCells[1].Value}");

            workbook.Save("ScenarioInputCellCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


