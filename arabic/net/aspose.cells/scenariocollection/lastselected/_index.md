---
title: "ScenarioCollection.LastSelected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScenarioCollection. تشير إلى أي سيناريو تم اختياره آخرًا من قبل المستخدم لتشغيله/عرضه"
type: docs
url: /ar/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

يشير إلى أي سيناريو تم اختياره آخر مرة من قبل المستخدم لتشغيله/عرضه.

```csharp
public int LastSelected { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف السيناريوهات
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // عيّن السيناريو النشط والفهرس المختار آخرًا
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // تحقق وعرض خاصية LastSelected
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // تعديل الفهرس المختار آخرًا
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### انظر أيضًا

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


