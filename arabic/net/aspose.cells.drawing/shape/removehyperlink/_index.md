---
title: "Shape.RemoveHyperlink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تزيل الارتباط التشعبي للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

يزيل الارتباط التشعبي للشكل.

```csharp
public void RemoveHyperlink()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل وتعيين الارتباط التشعبي
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // إزالة الارتباط التشعبي
            shape.RemoveHyperlink();

            // تحقق من إزالة الارتباط التشعبي
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // احفظ المصنف
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


