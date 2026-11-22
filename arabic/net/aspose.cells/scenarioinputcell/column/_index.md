---
title: "ScenarioInputCell.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioInputCell. تحصل وتعيّن فهرس العمود للخلية المدخلة"
type: docs
url: /ar/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

يحصل على ويضبط فهرس العمود للخلية المدخلة.

```csharp
public int Column { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
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

            // الوصول وعرض خاصية Column
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // نظرًا لأن Column للقراءة فقط، نحتاج إلى إزالته وإعادة إضافته لتغيير العمود
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // تحقق من التغيير
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // احفظ المصنف
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


