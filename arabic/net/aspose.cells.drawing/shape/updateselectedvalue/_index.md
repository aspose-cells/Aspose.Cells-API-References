---
title: "Shape.UpdateSelectedValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. قم بتحديث القيمة المحددة بقيمة الخلية المرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

حدّث القيمة المحددة بقيمة الخلية المرتبطة.

```csharp
public void UpdateSelectedValue()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // إنشاء شكل ListBox
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // تعيين نطاق الإدخال والخلية المرتبطة
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // الحصول على كائن ListBox
            ListBox listBox = (ListBox)listBoxShape;

            // تعيين القيمة الأولية في الخلية المرتبطة وتحديث الاختيار
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // تحقق من الاختيار
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // تغيير القيمة وتحديث الاختيار مرة أخرى
            worksheet.Cells["A12"].Value = 4;
            listBoxShape.UpdateSelectedValue();

            if (listBox.IsSelected(3))
            {
                Console.WriteLine("Option 4 is selected");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


