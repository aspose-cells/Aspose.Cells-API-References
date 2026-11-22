---
title: "Protection.AllowEditingObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان يُسمح للمستخدم بالتلاعب بأجسام الرسم في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع كائنات الرسم في ورقة عمل محمية.

```csharp
public bool AllowEditingObject { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ضبط إعدادات الحماية مع تمكين AllowEditingObject
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // تحقق من أعلام الحماية
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // إنشاء صندوق نص (كائن) لاختبار التحرير
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // احفظ المصنف
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


