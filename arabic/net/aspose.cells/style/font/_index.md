---
title: "Style.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل على كائن Font"
type: docs
url: /ar/net/aspose.cells/style/font/
---
## Style.Font property

يحصل على كائن `Font`.

```csharp
public Font Font { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // الوصول إلى الخلية B4 وتعيين الخط إلى غامق
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // الوصول إلى الخلية C4 والتأكد من أن الخط ليس غامقًا
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // الوصول إلى الخلية D4 وتعيين الخط إلى غامق بلون مختلف
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // تحقق من خصائص الخط
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // احفظ المصنف
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


