---
title: "Column.HasCustomStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. تشير إلى ما إذا كان لهذا العمود إعدادات نمط مخصصة تختلف عن النمط الافتراضي الموروث من المصنف"
type: docs
url: /ar/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

يشير إلى ما إذا كان هذا العمود يحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من المصنف).

```csharp
public bool HasCustomStyle { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى العمود الأول
            Column column = worksheet.Cells.Columns[0];

            // عرض قيمة HasCustomState الأولية
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // تعديل نمط العمود لتوضيح تغيير HasCustomStyle
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // عرض قيمة HasCustomStyle المحدثة
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // إنشاء عمود آخر بالنمط الافتراضي للمقارنة
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // احفظ المصنف
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


