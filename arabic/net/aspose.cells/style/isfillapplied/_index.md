---
title: "Style.IsFillApplied"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان يجب تطبيق تنسيق التعبئة"
type: docs
url: /ar/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

يشير إلى ما إذا كان يجب تطبيق تنسيق التعبئة.

```csharp
public bool IsFillApplied { get; set; }
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
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط
            Style style = workbook.CreateStyle();
            
            // في البداية، يجب أن يكون IsFillApplied false
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // تطبيق إعدادات التعبئة
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // بعد ضبط خصائص التعبئة، يجب أن يكون IsFillApplied true
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // تطبيق النمط على خلية
            worksheet.Cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


