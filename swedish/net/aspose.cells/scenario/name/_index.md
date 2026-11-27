---
title: "Scenario.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Scenario-egenskap. Hämtar och anger namnet på scenariot"
type: docs
url: /sv/net/aspose.cells/scenario/name/
---
## Scenario.Name property

Hämtar och anger namnet på scenariot.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("InitialScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Demonstrera användning av Name‑egenskapen
            Console.WriteLine("Original scenario name: " + scenario.Name);
            scenario.Name = "RenamedScenario";
            Console.WriteLine("Updated scenario name: " + scenario.Name);

            workbook.Save("ScenarioNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


