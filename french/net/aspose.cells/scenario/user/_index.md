---
title: "Scenario.User"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Scenario. Obtient le nom de l'utilisateur qui a modifié le scénario en dernier"
type: docs
url: /fr/net/aspose.cells/scenario/user/
---
## Scenario.User property

Obtient le nom de l'utilisateur qui a modifié le scénario en dernier.

```csharp
public string User { get; }
```

### Exemples

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

            // Démontrer l'utilisation de la propriété User
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


