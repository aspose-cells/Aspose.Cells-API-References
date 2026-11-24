---
title: "ScenarioCollection.ActiveIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioCollection-Eigenschaft. Liest und setzt, welches Szenario ausgewählt ist"
type: docs
url: /de/net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

Liest und setzt, welches Szenario ausgewählt ist.

```csharp
public int ActiveIndex { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyActiveIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");
            
            scenarios.ActiveIndex = scenarioIndex;
            
            Console.WriteLine($"Active scenario index set to: {scenarios.ActiveIndex}");
            
            workbook.Save("ScenarioActiveIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


