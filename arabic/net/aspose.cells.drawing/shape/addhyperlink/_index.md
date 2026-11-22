---
title: "Shape.AddHyperlink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تضيف ارتباطًا تشعبيًا إلى الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

يضيف ارتباطًا تشعبيًا إلى الشكل.

```csharp
public Hyperlink AddHyperlink(string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| address | String | عنوان الارتباط التشعبي. |

### قيمة الإرجاع

يرجع كائن الارتباط التشعبي الجديد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // أضف ارتباطًا تشعبيًا إلى الشكل باستخدام سلسلة URL
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // احفظ المصنف
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


