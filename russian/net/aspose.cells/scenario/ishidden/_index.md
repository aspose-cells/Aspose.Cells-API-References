---
title: "Scenario.IsHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Scenario. Указывает, скрыт ли сценарий"
type: docs
url: /ru/net/aspose.cells/scenario/ishidden/
---
## Scenario.IsHidden property

Указывает, скрыт ли сценарий.

```csharp
public bool IsHidden { get; set; }
```

### Примеры

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
            
            // Продемонстрировать свойство IsHidden
            scenario.IsHidden = true;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            scenario.IsHidden = false;
            Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
            
            workbook.Save("ScenarioIsHiddenDemo.xlsx");
        }
    }
}
```

### См. также

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


