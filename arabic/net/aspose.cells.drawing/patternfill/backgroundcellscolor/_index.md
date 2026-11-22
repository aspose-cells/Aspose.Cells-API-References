---
title: "PatternFill.BackgroundCellsColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PatternFill. تحصل وتعيّن كائن CellsColor الأمامي"
type: docs
url: /ar/net/aspose.cells.drawing/patternfill/backgroundcellscolor/
---
## PatternFill.BackgroundCellsColor property

تحصل وتعيّن كائن الـ [`CellsColor`](../../../aspose.cells/cellscolor/) الأمامي.

```csharp
public CellsColor BackgroundCellsColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackgroundCellsColorDemo
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

                // الوصول إلى خصائص BackgroundCellsColor وتعديلها
                patternFill.BackgroundCellsColor.Color = Color.Blue;
                patternFill.BackgroundCellsColor.Argb = Color.Blue.ToArgb();
                patternFill.BackgroundCellsColor.Transparency = 0.3;

                // عرض خصائص BackgroundCellsColor
                Console.WriteLine("BackgroundCellsColor Type: " + patternFill.BackgroundCellsColor.Type);
                Console.WriteLine("BackgroundCellsColor Color: " + patternFill.BackgroundCellsColor.Color);
                Console.WriteLine("BackgroundCellsColor ARGB: " + patternFill.BackgroundCellsColor.Argb);
                Console.WriteLine("BackgroundCellsColor Transparency: " + patternFill.BackgroundCellsColor.Transparency);

                // احفظ المصنف
                workbook.Save("BackgroundCellsColorDemo.xlsx");
                Console.WriteLine("BackgroundCellsColor demonstration completed successfully.");
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


