---
title: "الفئة Scenario"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Scenario. تمثل سيناريو فردي"
type: docs
url: /ar/net/aspose.cells/scenario/
---
## Scenario class

يمثل سيناريوًا فرديًا.

```csharp
public class Scenario
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | يحصل ويضبط تعليق السيناريو. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | يحصل على خلايا الإدخال للسيناريو. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | يشير إلى ما إذا كان السيناريو مخفيًا. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | يشير إلى ما إذا كان السيناريو مقفلًا للتعديل عندما تكون الورقة محمية. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | يحصل ويضبط اسم السيناريو. |
| [User](../../aspose.cells/scenario/user/) { get; } | يحصل على اسم المستخدم الذي قام بآخر تعديل للسيناريو. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى مجموعة السيناريوهات في ورقة العمل
            ScenarioCollection scenarios = worksheet.Scenarios;

            // أضف سيناريو جديد إلى المجموعة
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // ضبط خصائص السيناريو
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // الوصول إلى الخصائص للقراءة فقط
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // احفظ المصنف
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


