---
title: "Scenario.User"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Scenario özelliği. Senaryoyu en son değiştiren kullanıcının adını alır"
type: docs
url: /tr/net/aspose.cells/scenario/user/
---
## Scenario.User property

Senaryoyu en son değiştiren kullanıcının adını alır.

```csharp
public string User { get; }
```

### Örnekler

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

            // User özelliği kullanımını gösterin
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


