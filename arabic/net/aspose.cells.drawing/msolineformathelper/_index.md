---
title: "فئة MsoLineFormatHelper"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.MsoLineFormatHelper. تمثل تنسيق الخط ورأس السهم"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

يمثل تنسيق الخط ورأس السهم.

```csharp
public class MsoLineFormatHelper
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | يحصل على ويضبط لون خلفية خط الحدود. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | يحصل على أو يضبط نمط الشرط للخط المحدد. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | يحصل على ويضبط لون مقدمة خط الحدود. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | يشير إلى ما إذا كان الكائن مرئياً. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | يرجع كائن Style يمثل نمط النطاق المحدد. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | إرجاع أو تعيين درجة الشفافية للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | إرجاع أو تعيين وزن الخط، بوحدات النقاط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء شكل لتوضيح تنسيق الخط
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // الحصول على تنسيق الخط مباشرةً من الشكل
                MsoLineFormat lineFormat = shape.LineFormat;

                // تعيين الخصائص مباشرةً على تنسيق الخط
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // عرض الخصائص المُكوَّنة
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // احفظ المصنف
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


