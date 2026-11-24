---
title: "Scenario.IsHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Scenario-Eigenschaft. Gibt an, ob das Szenario ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/scenario/ishidden/
---
## Scenario.IsHidden property

Gibt an, ob das Szenario ausgeblendet ist.

```csharp
public bool IsHidden { get; set; }
```

### Beispiele

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
            
            // Demonstriere die IsHidden-Eigenschaft
            scenario.IsHidden = true;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            scenario.IsHidden = false;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            workbook.Save("ScenarioIsHiddenDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


