---
title: "UnionRange.FirstColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. تحصل على فهرس العمود الأول للنطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/firstcolumn/
---
## UnionRange.FirstColumn property

يحصل على فهرس العمود الأول في النطاق.

```csharp
public int FirstColumn { get; }
```

### ملاحظات

يؤثر فقط عندما يحتوي على نطاق واحد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // إنشاء نطاق اتحاد
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A2:C2");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // عرض خاصية FirstColumn
            Console.WriteLine("First column index of the union range: " + unionRange.FirstColumn);

            // إظهار استخدام FirstColumn في العمليات
            Console.WriteLine("First column name: " + CellsHelper.ColumnIndexToName(unionRange.FirstColumn));

            // تطبيق تنسيق على العمود الأول من نطاق الاتحاد
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstColumnRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow, unionRange.FirstColumn,
                unionRange.RowCount, 1);
            firstColumnRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // حفظ النتيجة
            workbook.Save("UnionRangePropertyFirstColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


