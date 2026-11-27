---
title: "Scenario.IsLocked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Scenario-egenskap. Anger om scenariot är låst för redigering när bladet är skyddat"
type: docs
url: /sv/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Anger om scenariot är låst för redigering när bladet är skyddat.

```csharp
public bool IsLocked { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("LockedScenario");
            Scenario scenario = scenarios[scenarioIndex];

            scenario.IsLocked = true;
            Console.WriteLine("Scenario locked status: " + scenario.IsLocked);

            workbook.Save("ScenarioLockDemo.xlsx");
        }
    }
}
```

### Se även

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


