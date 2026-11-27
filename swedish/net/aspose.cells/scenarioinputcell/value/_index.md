---
title: "ScenarioInputCell.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioInputCell-egenskapen. Hämtar och anger värdet för inmatningscellen"
type: docs
url: /sv/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Hämtar och anger värdet för indatacellen.

```csharp
public string Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett scenario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Lägg till inmatningsceller med värden
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Kom åt och ändra värden
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Spara arbetsboken
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


