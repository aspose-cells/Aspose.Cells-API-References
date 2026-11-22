---
title: "Protection.AllowEditingContent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان يُسمح للمستخدم بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

يمثل ما إذا كان يُسمح للمستخدم بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية.

```csharp
public bool AllowEditingContent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احمِ ورقة العمل باستخدام كلمة مرور
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // تحقق واعرض خاصية AllowEditingContent
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // عدّل خاصية AllowEditingContent
            worksheet.Protection.AllowEditingContent = true;
            
            // تحقق واعرض الخاصية المحدثة
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // احفظ المصنف
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


