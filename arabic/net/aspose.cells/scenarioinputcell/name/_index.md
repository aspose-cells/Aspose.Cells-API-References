---
title: "ScenarioInputCell.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioInputCell. تحصل وتعيّن عنوان الخلية المدخلة"
type: docs
url: /ar/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

يحصل على ويضبط عنوان الخلية المدخلة.

```csharp
public string Name { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء سيناريو
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // الحصول على السيناريو
            Scenario scenario = scenarios[scenarioIndex];

            // إضافة خلايا الإدخال إلى السيناريو
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // الحصول على خلايا الإدخال
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // عرض استخدام خاصية Name
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // تحقق من أن الأسماء تطابق القيم المتوقعة
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


