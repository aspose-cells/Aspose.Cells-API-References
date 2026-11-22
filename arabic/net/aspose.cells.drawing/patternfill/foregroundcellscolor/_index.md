---
title: "PatternFill.ForegroundCellsColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PatternFill. تحصل وتعيّن كائن CellsColor الأمامي"
type: docs
url: /ar/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

تحصل وتعيّن كائن الـ [`CellsColor`](../../../aspose.cells/cellscolor/) الأمامي.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل مستطيل لتوضيح تعبئة النمط
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // عيّن نوع التعبئة إلى نمط
                shape.Fill.FillType = FillType.Pattern;

                // احصل على نسخة PatternFill
                PatternFill patternFill = shape.Fill.PatternFill;

                // عيّن نوع النمط والألوان
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // إنشاء كائن CellsColor للمقدمة باستخدام خاصية Color
                // نظرًا لأن CellsColor لا يحتوي على مُنشئ عام، سنستخدم ForegroundCellsColor الموجود
                // وتعديل خصائصه مباشرةً
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // عرض خصائص ForegroundCellsColor
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // احفظ المصنف
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


