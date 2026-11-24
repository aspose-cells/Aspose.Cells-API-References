---
title: "Scenario.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Scenario-Eigenschaft. Gibt den Namen des Szenarios zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/scenario/name/
---
## Scenario.Name property

Liest und setzt den Namen des Szenarios.

```csharp
public string Name { get; set; }
```

### Beispiele

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

            // Demonstrieren Sie die Verwendung der Name-Eigenschaft
            Console.WriteLine("Original scenario name: " + scenario.Name);
            scenario.Name = "RenamedScenario";
            Console.WriteLine("Updated scenario name: " + scenario.Name);

            workbook.Save("ScenarioNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


