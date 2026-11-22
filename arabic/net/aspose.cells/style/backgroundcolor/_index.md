---
title: "Style.BackgroundColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل أو تعيّن لون خلفية النمط"
type: docs
url: /ar/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

يحصل على لون الخلفية للنمط أو يضبطه.

```csharp
public Color BackgroundColor { get; set; }
```

### ملاحظات

إذا كنت تريد تعيين لون الخلية، يرجى استخدام خاصية Style.ForegroundColor. سيتفعّل هذا الخصائص فقط إذا كان نمط خلية النمط غير 'none' أو 'solid'.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء كائن نمط
            Style style = workbook.CreateStyle();
            
            // عيّن لون الخلفية إلى الأصفر
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // تطبيق النمط على الخلية A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


