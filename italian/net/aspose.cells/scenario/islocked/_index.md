---
title: "Scenario.IsLocked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Scenario. Indica se lo scenario è bloccato per la modifica quando il foglio è protetto"
type: docs
url: /it/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Indica se lo scenario è bloccato per la modifica quando il foglio è protetto.

```csharp
public bool IsLocked { get; set; }
```

### Esempi

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

### Vedi anche

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


