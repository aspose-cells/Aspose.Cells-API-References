---
title: "Scenario.User"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Scenario. تحصل على اسم المستخدم الذي قام بآخر تعديل للسيناريو"
type: docs
url: /ar/net/aspose.cells/scenario/user/
---
## Scenario.User property

يحصل على اسم المستخدم الذي قام بآخر تعديل للسيناريو.

```csharp
public string User { get; }
```

### أمثلة

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

            // عرض استخدام خاصية User
            Console.WriteLine("Scenario created by user: " + scenario.User);

            workbook.Save("ScenarioUserDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


