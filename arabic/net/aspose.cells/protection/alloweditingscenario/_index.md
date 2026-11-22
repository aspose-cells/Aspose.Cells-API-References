---
title: "Protection.AllowEditingScenario"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان يُسمح للمستخدم بتحرير السيناريوهات في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

يمثل ما إذا كان يُسمح للمستخدم بتحرير السيناريوهات في ورقة عمل محمية.

```csharp
public bool AllowEditingScenario { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // الوصول إلى إعدادات حماية ورقة العمل
            Protection protection = worksheet.Protection;

            // ضبط خصائص الحماية مع تمكين AllowEditingScenario
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);

            // احفظ المصنف
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


