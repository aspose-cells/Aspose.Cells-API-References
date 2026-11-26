---
title: "Scenario.IsLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Scenario. Indica si el escenario está bloqueado para edición cuando la hoja está protegida"
type: docs
url: /es/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Indica si el escenario está bloqueado para edición cuando la hoja está protegida.

```csharp
public bool IsLocked { get; set; }
```

### Ejemplos

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

### Ver también

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


