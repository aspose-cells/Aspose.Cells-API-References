---
title: "ScenarioCollection.ActiveIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioCollection. تحصل وتعيّن أي سيناريو تم اختياره"
type: docs
url: /ar/net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

يحصل على ويضبط أي سيناريو تم اختياره.

```csharp
public int ActiveIndex { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyActiveIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");
            
            scenarios.ActiveIndex = scenarioIndex;
            
            Console.WriteLine($"Active scenario index set to: {scenarios.ActiveIndex}");
            
            workbook.Save("ScenarioActiveIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


