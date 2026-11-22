---
title: "LineFormat.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LineFormat. تحدد ما إذا كانت هذه المثيلة لها نفس القيمة مثل كائن LineFormat المحدد الآخر"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

تحدد ما إذا كانت هذه المثيلة لها نفس القيمة مثل كائن [`LineFormat`](../) المحدد الآخر.

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | كائن [`LineFormat`](../) للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

صحيح إذا كانت قيمة المعامل obj هي نفسها قيمة هذه المثيلة؛ وإلا، خطأ. إذا كان obj فارغًا، تُعيد هذه الطريقة خطأ.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكل خط إلى ورقة العمل
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // احصل على تنسيق الخط للشكل الأول
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // قارن تنسيقات الخط باستخدام طريقة Equals
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### انظر أيضًا

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


