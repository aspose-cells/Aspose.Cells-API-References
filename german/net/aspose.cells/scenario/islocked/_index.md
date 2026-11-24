---
title: "Scenario.IsLocked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Scenario-Eigenschaft. Gibt an, ob das Szenario beim geschützten Blatt für die Bearbeitung gesperrt ist"
type: docs
url: /de/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Gibt an, ob das Szenario beim geschützten Blatt für die Bearbeitung gesperrt ist.

```csharp
public bool IsLocked { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


