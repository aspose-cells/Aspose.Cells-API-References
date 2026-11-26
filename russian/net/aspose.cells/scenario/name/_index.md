---
title: "Scenario.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Scenario. Получает и задаёт имя сценария"
type: docs
url: /ru/net/aspose.cells/scenario/name/
---
## Scenario.Name property

Получает и задает имя сценария.

```csharp
public string Name { get; set; }
```

### Примеры

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

            // Продемонстрировать использование свойства Name
            Console.WriteLine("Original scenario name: " + scenario.Name);
            scenario.Name = "RenamedScenario";
            Console.WriteLine("Updated scenario name: " + scenario.Name);

            workbook.Save("ScenarioNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


