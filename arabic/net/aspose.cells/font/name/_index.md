---
title: "Font.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. الحصول على أو تعيين اسم الخط"
type: docs
url: /ar/net/aspose.cells/font/name/
---
## Font.Name property

الحصول على أو تعيين اسم [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### ملاحظات

إذا تم استخدام هذه الخاصية لتعيين اسم الخط، سيتم تحديث [`SchemeType`](../schemetype/) إلى None

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الافتراضية والخلايا
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // إنشاء وتعديل نمط بخصائص الخط
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // عرض استخدام خاصية Name
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // تطبيق النمط على خلية
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


