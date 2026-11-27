---
title: "Scenario.User"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Scenario-egenskap. Hämtar namnet på användaren som senast ändrade scenariot"
type: docs
url: /sv/net/aspose.cells/scenario/user/
---
## Scenario.User property

Hämtar namnet på den användare som senast ändrade scenariot.

```csharp
public string User { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyUserDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Demonstrera användning av User-egenskapen
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### Se även

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


