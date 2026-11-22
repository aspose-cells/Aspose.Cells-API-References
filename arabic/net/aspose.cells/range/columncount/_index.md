---
title: "Range.ColumnCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تُعيد عدد الأعمدة في النطاق"
type: docs
url: /ar/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

يحصل على عدد الأعمدة في النطاق.

```csharp
public int ColumnCount { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // أنشئ بيانات نموذجية (5 أعمدة × 3 صفوف)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // أنشئ نطاقًا يغطي جميع أعمدة البيانات
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // أظهر استخدام ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // اضبط تلقائيًا كل عمود في النطاق
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


