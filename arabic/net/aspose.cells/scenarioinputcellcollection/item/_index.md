---
title: "ScenarioInputCellCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioInputCellCollection. تحصل على ScenarioInputCell حسب الفهرس في القائمة"
type: docs
url: /ar/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

يحصل على [`ScenarioInputCell`](../../scenarioinputcell/) حسب الفهرس في القائمة.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس المحدد في القائمة |

### قيمة الإرجاع

الكائن [`ScenarioInputCell`](../../scenarioinputcell/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            // عرض استخدام خاصية Item
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


