---
title: "Row.HasCustomStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تشير إلى ما إذا كان لهذا الصف إعدادات نمط مخصصة تختلف عن النمط الافتراضي الموروث من المصنف"
type: docs
url: /ar/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

يشير إلى ما إذا كان هذا الصف يحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من المصنف).

```csharp
public bool HasCustomStyle { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء وتخصيص نمط
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // الوصول إلى الصف الأول
            Row row = worksheet.Cells.Rows[0];
            
            // تطبيق نمط مخصص على الصف
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // تحقق مما إذا كان الصف يحتوي على نمط مخصص (يجب أن يكون صحيحًا)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // احفظ المصنف
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


