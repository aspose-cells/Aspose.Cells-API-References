---
title: "Scenario.Comment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Scenario. تحصل على تعليق السيناريو وتعيينه"
type: docs
url: /ar/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

يحصل ويضبط تعليق السيناريو.

```csharp
public string Comment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة سيناريوهات
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // إضافة سيناريو
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // تعيين خصائص السيناريو
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // إضافة خلايا الإدخال إلى السيناريو باستخدام مراجع الخلايا والقيم
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // عرض تعليق السيناريو
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // احفظ المصنف
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


