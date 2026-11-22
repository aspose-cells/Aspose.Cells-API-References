---
title: "Shape.GetInputRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تسترجع النطاق المستخدم لملء التحكم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

يحصل على النطاق المستخدم لملء التحكم.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### قيمة الإرجاع

النطاق المستخدم لملء التحكم.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // أضف شكل صندوق قائمة
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // حدد النطاق الإدخالي لصندوق القائمة
            shape.SetInputRange("$A$1:$A$3", false, false);

            // احصل على النطاق الإدخالي
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


