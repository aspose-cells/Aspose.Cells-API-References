---
title: "الفئة ColorFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.ColorFilter. يمثل إعدادًا لتصفية النطاق حسب اللون"
type: docs
url: /ar/net/aspose.cells/colorfilter/
---
## ColorFilter class

يمثل إعدادًا لتصفية النطاق حسب اللون.

```csharp
public class ColorFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FilterByFillColor](../../aspose.cells/colorfilter/filterbyfillcolor/) { get; set; } | ما إذا كان يتم التصفية حسب لون تعبئة الخلية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetColor](../../aspose.cells/colorfilter/getcolor/)(WorksheetCollection) | يحصل على لون هذا الفلتر. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassColorFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة بألوان مختلفة
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Red");
            cells["A2"].PutValue("Green");
            cells["A3"].PutValue("Blue");
            cells["A4"].PutValue("Red");
            
            // تطبيق الألوان على الخلايا
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A1"].SetStyle(style1);
            cells["A4"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Green;
            style2.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = Color.Blue;
            style3.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style3);
            
            // إنشاء مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // إنشاء فلتر لون للخلايا الحمراء
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, cr, cr);
            filter.Refresh();
            
            // تحقق من الصفوف المصفاة
            Console.WriteLine("Row 1 hidden: " + cells.IsRowHidden(0));
            Console.WriteLine("Row 2 hidden: " + cells.IsRowHidden(1));
            Console.WriteLine("Row 3 hidden: " + cells.IsRowHidden(2));
            Console.WriteLine("Row 4 hidden: " + cells.IsRowHidden(3));
            
            // الوصول إلى فلتر اللون
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            Console.WriteLine("Filter by fill color: " + cf.FilterByFillColor);
            Console.WriteLine("Filter color: " + cf.GetColor(workbook.Worksheets));
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


