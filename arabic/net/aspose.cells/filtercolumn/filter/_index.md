---
title: "FilterColumn.Filter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. تحصل وتضبط شرط تصفية البيانات"
type: docs
url: /ar/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

تحصل وتضبط شرط تصفية البيانات.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام الخاصية المقابلة وفقًا لـ [`FilterType`](../filtertype/). ولنوع الفلتر MultipleFilters، الكائن المرتجع هو الآن [`FilterValueCollection`](../../filtervaluecollection/) بدلاً من [`MultipleFilterCollection`](../../multiplefiltercollection/). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية مع تنسيق اللون
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // تنسيق الخلايا بالألوان
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // إضافة فلتر لون للخلايا الحمراء
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // الوصول إلى عمود الفلتر وخاصية Filter الخاصة به
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // إخراج خصائص الفلتر
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // احفظ المصنف
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


