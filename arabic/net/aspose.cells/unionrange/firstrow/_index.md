---
title: "UnionRange.FirstRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. يحصل على فهرس الصف الأول للنطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/firstrow/
---
## UnionRange.FirstRow property

يحصل على فهرس الصف الأول في النطاق.

```csharp
public int FirstRow { get; }
```

### ملاحظات

يؤثر فقط عندما يحتوي على نطاق واحد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
                }
            }

            // إنشاء نطاق اتحاد من A2:C5 و A7:C9
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // عرض خاصية FirstRow
            Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);

            // إظهار الاستخدام عن طريق تمييز الصف الأول
            Style highlightStyle = workbook.CreateStyle();
            highlightStyle.Font.IsBold = true;
            highlightStyle.ForegroundColor = System.Drawing.Color.LightGreen;
            highlightStyle.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstRowRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow,
                unionRange.FirstColumn,
                1,
                unionRange.ColumnCount);
            firstRowRange.ApplyStyle(highlightStyle, new StyleFlag { FontBold = true, CellShading = true });

            // إنشاء نطاق آخر ومقارنة قيم FirstRow
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
            Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
            Console.WriteLine("Is union range starting after single range? " + 
                (unionRange.FirstRow > singleRange.FirstRow));

            // احفظ المصنف
            workbook.Save("UnionRangeFirstRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


