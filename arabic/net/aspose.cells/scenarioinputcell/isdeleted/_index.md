---
title: "ScenarioInputCell.IsDeleted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioInputCell. تشير إلى ما إذا كانت الخلية المدخلة محذوفة"
type: docs
url: /ar/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

يشير إلى ما إذا كانت الخلية المدخلة محذوفة.

```csharp
public bool IsDeleted { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة سيناريو
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // إضافة خلايا الإدخال
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // الوصول وعرض خلايا الإدخال
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // حذف الخلية المدخلة الأولى
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // احفظ المصنف
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


