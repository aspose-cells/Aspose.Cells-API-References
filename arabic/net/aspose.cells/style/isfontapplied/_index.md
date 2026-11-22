---
title: "Style.IsFontApplied"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان يجب تطبيق تنسيق الخط"
type: docs
url: /ar/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

يشير إلى ما إذا كان يجب تطبيق تنسيق الخط.

```csharp
public bool IsFontApplied { get; set; }
```

### ملاحظات

فقط للنمط المسمى.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى خلية من ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // احصل على نمط الخلية
            Style style = cell.GetStyle();
            
            // تطبيق إعدادات الخط
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // تمكين تطبيق الخط
            style.IsFontApplied = true;
            
            // إعادة النمط المعدل إلى الخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


