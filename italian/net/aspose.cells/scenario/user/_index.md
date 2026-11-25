---
title: "Scenario.User"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Scenario. Ottiene il nome dell'utente che ha modificato per ultimo lo scenario"
type: docs
url: /it/net/aspose.cells/scenario/user/
---
## Scenario.User property

Ottiene il nome dell'utente che ha modificato per ultimo lo scenario.

```csharp
public string User { get; }
```

### Esempi

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

            // Dimostra l'uso della proprietà User
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


