---
title: "Scenario.IsLocked"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Scenario özelliği. Sayfa korunduğunda senaryonun düzenleme için kilitli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Sayfa korunduğunda senaryonun düzenleme için kilitli olup olmadığını gösterir.

```csharp
public bool IsLocked { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


