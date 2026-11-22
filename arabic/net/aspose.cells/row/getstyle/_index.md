---
title: "Row.GetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. تحصل على نمط هذا الصف"
type: docs
url: /ar/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

يسترجع نمط هذا الصف.

```csharp
public Style GetStyle()
```

### ملاحظات

تعديل كائن النمط المرتجع مباشرة لا يؤثر على هذا الصف أو أي خلايا فيه. عليك استدعاء طريقة [`ApplyStyle`](../applystyle/) أو طريقة [`SetStyle`](../setstyle/) لتطبيق التغيير على هذا الصف. نمط الصف هو النمط الذي سيُورث إلى الخلايا في هذا الصف (تلك الخلايا التي لا تحتوي على إعدادات نمط مخصصة، مثل الخلايا الموجودة التي لم يتم تعيين نمط لها صراحةً، أو تلك التي لم يتم إنشاءها).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين الأنماط للعرض
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // عرض استخدام GetStyle
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


