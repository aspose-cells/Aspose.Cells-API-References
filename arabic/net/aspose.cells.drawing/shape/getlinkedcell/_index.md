---
title: "Shape.GetLinkedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تحصل على النطاق المرتبط بقيمة التحكم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

يحصل على النطاق المرتبط بقيمة التحكم.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### قيمة الإرجاع

النطاق المرتبط بقيمة التحكم.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل وتعيين الخلية المرتبطة به
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.LinkedCell = "A1";

            // الحصول على عنوان الخلية المرتبطة باستخدام تركيبات مختلفة من المعلمات
            string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
            string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
            string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference

            Console.WriteLine("Linked cell (absolute A1): " + link1);
            Console.WriteLine("Linked cell (relative A1): " + link2);
            Console.WriteLine("Linked cell (R1C1 style): " + link3);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


