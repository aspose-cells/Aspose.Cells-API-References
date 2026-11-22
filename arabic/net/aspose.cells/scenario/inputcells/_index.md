---
title: "Scenario.InputCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Scenario. تحصل على خلايا الإدخال للسيناريو"
type: docs
url: /ar/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

يحصل على خلايا الإدخال للسيناريو.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة سيناريو إلى ورقة العمل
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // إضافة خلايا الإدخال إلى السيناريو باستخدام خاصية InputCells
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // تعديل قيمة خلية الإدخال الأولى
            inputCells[0].Value = "150";

            // احفظ المصنف
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


