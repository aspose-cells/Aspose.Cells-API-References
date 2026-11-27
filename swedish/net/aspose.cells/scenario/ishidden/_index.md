---
title: "Scenario.IsHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Scenario-egenskap. Anger om scenariot är dolt"
type: docs
url: /sv/net/aspose.cells/scenario/ishidden/
---
## Scenario.IsHidden property

Anger om scenariot är dolt.

```csharp
public bool IsHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyIsHiddenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ScenarioCollection scenarios = worksheet.Scenarios;
            int index = scenarios.Add("TestScenario");
            Scenario scenario = scenarios[index];
            
            // Demonstrera IsHidden-egenskapen
            scenario.IsHidden = true;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            scenario.IsHidden = false;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            workbook.Save("ScenarioIsHiddenDemo.xlsx");
        }
    }
}
```

### Se även

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


