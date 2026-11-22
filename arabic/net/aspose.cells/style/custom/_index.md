---
title: "Style.Custom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تمثل سلسلة تنسيق الرقم المخصص لهذا الكائن النمطي. إذا لم يتم تعيين تنسيق الرقم المخصص، على سبيل المثال سيتم إرجاع تنسيق الرقم المدمج"
type: docs
url: /ar/net/aspose.cells/style/custom/
---
## Style.Custom property

يمثل سلسلة تنسيق الرقم المخصص لهذا الكائن من النوع Style. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، إذا كان تنسيق الرقم مدمجًا)، سيتم إرجاع "".

```csharp
public string Custom { get; set; }
```

### ملاحظات

السلسلة المخصصة المرتجعة مستقلة عن الثقافة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء وتطبيق تنسيق تاريخ مخصص
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // عرض القيمة المنسقة
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // احفظ المصنف
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


