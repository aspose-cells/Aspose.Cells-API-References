---
title: "Scenario.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Scenario. تحصل على اسم السيناريو وتعيينه"
type: docs
url: /ar/net/aspose.cells/scenario/name/
---
## Scenario.Name property

يحصل ويضبط اسم السيناريو.

```csharp
public string Name { get; set; }
```

### أمثلة

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

            // عرض استخدام خاصية Name
            Console.WriteLine("Original scenario name: " + scenario.Name);
            scenario.Name = "RenamedScenario";
            Console.WriteLine("Updated scenario name: " + scenario.Name);

            workbook.Save("ScenarioNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


