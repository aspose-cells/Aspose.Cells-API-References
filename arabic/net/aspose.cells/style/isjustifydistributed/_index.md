---
title: "Style.IsJustifyDistributed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان يجب استخدام محاذاة مبررة أو موزعة للخلية في السطر الأخير من النص"
type: docs
url: /ar/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

يشير إلى ما إذا كان يجب استخدام محاذاة مبررة أو موزعة للخلية في السطر الأخير من النص.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### ملاحظات

هذا شائع لتنسيقات شرق آسيا لكنه غير شائع في سياقات أخرى. يعمل فقط عندما تكون المحاذاة موزعة أفقياً.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية B3 وتعيين نصها
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // احصل على نمط الخلية وعيّن IsJustifyDistributed إلى true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحقق من الخاصية
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


