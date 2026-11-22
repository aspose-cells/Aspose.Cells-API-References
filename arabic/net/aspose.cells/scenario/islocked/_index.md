---
title: "Scenario.IsLocked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Scenario. تشير إلى ما إذا كان السيناريو مقفلاً للتحرير عندما تكون الورقة محمية"
type: docs
url: /ar/net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

يشير إلى ما إذا كان السيناريو مقفلًا للتعديل عندما تكون الورقة محمية.

```csharp
public bool IsLocked { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


