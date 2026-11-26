---
title: "Scenario.User"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Scenario. Получает имя пользователя, который последним изменил сценарий"
type: docs
url: /ru/net/aspose.cells/scenario/user/
---
## Scenario.User property

Получает имя пользователя, последним изменившего сценарий.

```csharp
public string User { get; }
```

### Примеры

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

            // Продемонстрировать использование свойства User
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### См. также

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


