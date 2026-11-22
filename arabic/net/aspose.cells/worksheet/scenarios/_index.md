---
title: "Worksheet.Scenarios"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. يحصل على مجموعة Scenario"
type: docs
url: /ar/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

يحصل على مجموعة [`Scenario`](../../scenario/).

```csharp
public ScenarioCollection Scenarios { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // أضف السيناريوهات
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // احفظ المصنف
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // امسح السيناريوهات واحفظ مرة أخرى
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


