---
title: "Scenario.IsHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Scenario. Indica se lo scenario è nascosto"
type: docs
url: /it/net/aspose.cells/scenario/ishidden/
---
## Scenario.IsHidden property

Indica se lo scenario è nascosto.

```csharp
public bool IsHidden { get; set; }
```

### Esempi

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
            
            // Dimostra la proprietà IsHidden
            scenario.IsHidden = true;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            scenario.IsHidden = false;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            workbook.Save("ScenarioIsHiddenDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


