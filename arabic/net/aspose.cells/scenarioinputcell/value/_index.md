---
title: "ScenarioInputCell.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioInputCell. يحصل على قيمة الخلية المدخلة ويضبطها"
type: docs
url: /ar/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

يحصل على ويضبط قيمة الخلية المدخلة.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة سيناريو
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // إضافة خلايا إدخال مع قيم
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // الوصول إلى القيم وتعديلها
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // احفظ المصنف
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


