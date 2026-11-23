---
title: "Scenario.IsLocked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Scenario. Indique si le scénario est verrouillé pour l'édition lorsque la feuille est protégée"
type: docs
url: /fr/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Indique si le scénario est verrouillé pour l'édition lorsque la feuille est protégée.

```csharp
public bool IsLocked { get; set; }
```

### Exemples

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

### Voir aussi

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


