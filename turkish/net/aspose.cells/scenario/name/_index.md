---
title: "Scenario.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Scenario özelliği. Senaryonun adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/scenario/name/
---
## Scenario.Name property

Senaryonun adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

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

            // Name özelliğinin kullanımını göster
            Console.WriteLine("Original scenario name: " + scenario.Name);
            scenario.Name = "RenamedScenario";
            Console.WriteLine("Updated scenario name: " + scenario.Name);

            workbook.Save("ScenarioNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


