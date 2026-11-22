---
title: "StyleFlag.LeftBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعدادات الحد الأيسر"
type: docs
url: /ar/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

سيتم تطبيق إعدادات الحد الأيسر.

```csharp
public bool LeftBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // إنشاء نطاق وتطبيق نمط الحد الأيسر
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // إنشاء نمط وعلم
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // تعيين خصائص الحد الأيسر
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // تطبيق النمط مع علم الحد الأيسر
            range.ApplyStyle(style, flag);

            // تحقق من تطبيق الحد الأيسر
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // احفظ المصنف
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


