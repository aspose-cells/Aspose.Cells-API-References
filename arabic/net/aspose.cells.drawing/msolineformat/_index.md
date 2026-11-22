---
title: "فئة MsoLineFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.MsoLineFormat. تمثل تنسيق الخط ورأس السهم"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

يمثل تنسيق الخط ورأس السهم.

```csharp
public class MsoLineFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | يحصل على ويضبط لون خلفية خط الحدود. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | يحصل على أو يضبط نمط الشرط للخط المحدد. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | يحصل على ويضبط لون مقدمة خط الحدود. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | يشير إلى ما إذا كان الكائن مرئياً. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | يرجع كائن Style يمثل نمط النطاق المحدد. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | إرجاع أو تعيين درجة الشفافية للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | إرجاع أو تعيين وزن الخط، بوحدات النقاط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // إنشاء كائن Workbook جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً قوسيًا إلى ورقة العمل
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // احصل على كائن MsoLineFormat من الشكل
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // ضبط خصائص كائن MsoLineFormat
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // احفظ المصنف
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


