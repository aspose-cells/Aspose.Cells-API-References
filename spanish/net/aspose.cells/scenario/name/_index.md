---
title: "Scenario.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Scenario. Obtiene y establece el nombre del escenario"
type: docs
url: /es/net/aspose.cells/scenario/name/
---
## Scenario.Name property

Obtiene y establece el nombre del escenario.

```csharp
public string Name { get; set; }
```

### Ejemplos

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

            // Demostrar el uso de la propiedad Name
            Console.WriteLine("Original scenario name: " + scenario.Name);
            scenario.Name = "RenamedScenario";
            Console.WriteLine("Updated scenario name: " + scenario.Name);

            workbook.Save("ScenarioNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


