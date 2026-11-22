---
title: "Worksheet.IsRulerVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Worksheet property. يشير إلى ما إذا كان المسطرة مرئية. يتم تطبيق هذه الخاصية فقط في معاينة فواصل الصفحات"
type: docs
url: /ar/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

يشير إلى ما إذا كان المسطرة مرئية. يتم تطبيق هذه الخاصية فقط في معاينة فواصل الصفحات.

```csharp
public bool IsRulerVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // اضبط الـ worksheet إلى PageLayoutView حيث تكون المسطرة مرئية
            worksheet.ViewType = ViewType.PageLayoutView;

            // بدّل إظهار المسطرة
            worksheet.IsRulerVisible = true;

            // أخرج حالة رؤية المسطرة الحالية
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // احفظ المصنف
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


