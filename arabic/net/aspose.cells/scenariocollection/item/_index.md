---
title: "ScenarioCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioCollection. تحصل على كائن Scenario حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

يحصل على كائن [`Scenario`](../../scenario/) حسب الفهرس.

```csharp
public Scenario this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس المحدد في القائمة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            scenario.InputCells.Add(0, 0, "100");
            scenario.InputCells.Add(1, 1, "200");

            // عرض استخدام خاصية Item
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


