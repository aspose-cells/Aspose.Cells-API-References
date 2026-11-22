---
title: "Shape.SetInputRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تعيين النطاق المستخدم لملء التحكم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

يضبط النطاق المستخدم لملء التحكم.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | النطاق المستخدم لملء التحكم. |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية إلى الخلايا A1:A10
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // أضف شكل صندوق قائمة
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // تعيين نطاق الإدخال لصندوق القائمة (باستخدام معلمات String, Boolean, Boolean)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // تعيين الخلية المرتبطة لصندوق القائمة
            listBox.SetLinkedCell("$A$12", false, true);

            // احفظ المصنف
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


