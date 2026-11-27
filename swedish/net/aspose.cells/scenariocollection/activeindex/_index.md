---
title: "ScenarioCollection.ActiveIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioCollection egenskap. Hämtar och anger vilket scenario som är valt"
type: docs
url: /sv/net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

Hämtar och anger vilket scenario som är valt.

```csharp
public int ActiveIndex { get; set; }
```

### Exempel

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

### Se även

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


