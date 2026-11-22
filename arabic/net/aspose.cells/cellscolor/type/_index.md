---
title: "CellsColor.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. نوع اللون"
type: docs
url: /ar/net/aspose.cells/cellscolor/type/
---
## CellsColor.Type property

نوع اللون.

```csharp
public ColorType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لتوضيح CellsColor
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            CellsColor cellsColor = shape.Fill.SolidFill.CellsColor;

            // عرض نوع اللون الأولي
            Console.WriteLine("Initial Color Type: " + cellsColor.Type);

            // تعيين لون RGB وإظهار تغيير النوع
            cellsColor.Color = System.Drawing.Color.Red;
            Console.WriteLine("After setting RGB Color - Type: " + cellsColor.Type);

            // تعيين لون مفهرس وإظهار تغيير النوع
            cellsColor.ColorIndex = 5; // Standard Excel color index
            Console.WriteLine("After setting ColorIndex - Type: " + cellsColor.Type);

            // تعيين لون السمة وإظهار تغيير النوع
            cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0); // Added tint parameter
            Console.WriteLine("After setting ThemeColor - Type: " + cellsColor.Type);

            // توضيح أنواع الألوان المختلفة في الخلايا
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("RGB Color");
            Style style1 = cell1.GetStyle(); // Use GetStyle() instead of Style property
            style1.ForegroundColor = System.Drawing.Color.Blue;
            style1.Pattern = BackgroundType.Solid;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Indexed Color");
            Style style2 = cell2.GetStyle(); // Use GetStyle() instead of Style property
            style2.ForegroundColor = System.Drawing.Color.FromArgb(5); // Using color index
            style2.Pattern = BackgroundType.Solid;
            cell2.SetStyle(style2);

            // حفظ النتيجة
            workbook.Save("CellsColorTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ColorType](../../colortype/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


