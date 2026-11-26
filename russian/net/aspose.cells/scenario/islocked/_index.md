---
title: "Scenario.IsLocked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Scenario. Указывает, заблокирован ли сценарий для редактирования, когда лист защищён"
type: docs
url: /ru/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Указывает, заблокирован ли сценарий для редактирования, когда лист защищён.

```csharp
public bool IsLocked { get; set; }
```

### Примеры

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

### См. также

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


