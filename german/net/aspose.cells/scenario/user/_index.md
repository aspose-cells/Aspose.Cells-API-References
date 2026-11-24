---
title: "Scenario.User"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Scenario-Eigenschaft. Gibt den Namen des Benutzers zurück, der das Szenario zuletzt geändert hat"
type: docs
url: /de/net/aspose.cells/scenario/user/
---
## Scenario.User property

Liest den Namen des Benutzers, der das Szenario zuletzt geändert hat.

```csharp
public string User { get; }
```

### Beispiele

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

            // Demonstriere die Verwendung der User-Eigenschaft
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


