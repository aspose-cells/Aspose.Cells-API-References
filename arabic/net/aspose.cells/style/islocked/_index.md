---
title: "Style.IsLocked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل أو تعين قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا"
type: docs
url: /ar/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

يحصل على قيمة أو يضبطها تشير إلى ما إذا كان يمكن تعديل الخلية أم لا.

```csharp
public bool IsLocked { get; set; }
```

### ملاحظات

قفل الخلايا لا يؤثر إلا إذا تم حماية ورقة العمل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين خاصية IsLocked لخلية
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // حماية ورقة العمل لفرض القفل
            worksheet.Protect(ProtectionType.All);

            // التحقق وطباعة حالة IsLocked
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // احفظ المصنف
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


