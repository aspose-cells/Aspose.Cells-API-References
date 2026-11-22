---
title: "الفئة Border"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Border. تغلف الكائن الذي يمثل حد الخلية"
type: docs
url: /ar/net/aspose.cells/border/
---
## Border class

يحتوي على الكائن الذي يمثل حد الخلية.

```csharp
public class Border
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | يحصل ويضبط اللون باستخدام قيمة ARGB ذات 32 بت. |
| [Color](../../aspose.cells/border/color/) { get; set; } | يحصل أو يضبط لون الحد. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | يحصل أو يضبط نوع حد الخلية. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | يحصل ويضبط لون السمة للحد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى كائن Workbook
            workbook.Worksheets.Add();

            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية "A1" من ورقة العمل
            Cell cell = worksheet.Cells["A1"];

            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Hello World");

            // الحصول على نمط الخلية
            Style style = cell.GetStyle();

            // ضبط نمط الخط للحد العلوي
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // ضبط نمط الخط للحد السفلي
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // ضبط نمط الخط للحد الأيسر
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // ضبط نمط الخط للحد الأيمن
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // حفظ ملف Excel
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


