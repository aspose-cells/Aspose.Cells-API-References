---
title: "ConditionalFormattingIcon.Index"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingIcon. يحصل على ويضبط فهرس الأيقونات في مجموعة الأيقونات"
type: docs
url: /ar/net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

يحصل ويعيّن فهرس الأيقونة في مجموعة الأيقونات.

```csharp
public int Index { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // إضافة تنسيق شرطي لمجموعة الأيقونات
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.IconSet);
            
            // تعيين خصائص مجموعة الأيقونات
            FormatCondition condition = fcc[0];
            condition.IconSet.Type = IconSetType.Arrows3;
            ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;

            // اعرض فهرس كل أيقونة
            Console.WriteLine("Icon Indexes:");
            for (int i = 0; i < icons.Count; i++)
            {
                Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
            }

            // عدّل وأظهر خاصية الفهرس
            icons[1].Index = 2;
            Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


