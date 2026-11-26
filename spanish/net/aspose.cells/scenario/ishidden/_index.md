---
title: "Scenario.IsHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Scenario. Indica si el escenario está oculto"
type: docs
url: /es/net/aspose.cells/scenario/ishidden/
---
## Scenario.IsHidden property

Indica si el escenario está oculto.

```csharp
public bool IsHidden { get; set; }
```

### Ejemplos

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
            
            // Demostrar la propiedad IsHidden
            scenario.IsHidden = true;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            scenario.IsHidden = false;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            workbook.Save("ScenarioIsHiddenDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


