---
title: "Cells.MaxDisplayRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. يحصل على النطاق الأقصى الذي يشمل الخلايا المدمجة والبيانات والأشكال"
type: docs
url: /ar/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

يحصل على النطاق الأقصى الذي يشمل البيانات والخلايا المدمجة والأشكال.

```csharp
public Range MaxDisplayRange { get; }
```

### ملاحظات

يرجع null إذا كانت ورقة العمل فارغة منذ Aspose.Cells 21.5.2.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى cells لإنشاء نطاق عرض
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // احصل على نطاق العرض الأقصى
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // إخراج معلومات النطاق
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // إنشاء range جديد بناءً على أبعاد نطاق العرض الأقصى
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // تطبيق التنسيق على range
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // احفظ المصنف
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


