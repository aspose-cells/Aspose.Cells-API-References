---
title: "Scenario.User"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Scenario. Obtiene el nombre del usuario que cambió el escenario por última vez"
type: docs
url: /es/net/aspose.cells/scenario/user/
---
## Scenario.User property

Obtiene el nombre del usuario que cambió el escenario por última vez.

```csharp
public string User { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyUserDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Demostrar el uso de la propiedad User
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


