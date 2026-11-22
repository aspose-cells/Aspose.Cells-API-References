---
title: "ScenarioInputCell.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioInputCell. تحصل وتعيّن فهرس الصف للخلية المدخلة"
type: docs
url: /ar/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

يحصل على ويضبط فهرس الصف للخلية المدخلة.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة سيناريو إلى ورقة العمل
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // إضافة خلايا الإدخال إلى السيناريو
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // الوصول وعرض خاصية Row
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // إضافة خلية جديدة في الصف 2 بدلاً من محاولة تعديل الموجودة
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // احفظ المصنف
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


