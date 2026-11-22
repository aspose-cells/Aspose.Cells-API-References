---
title: "الفئة Fill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Fill. تمثل تنسيق التعبئة للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/fill/
---
## Fill class

يمثل تنسيق التعبئة للشكل.

```csharp
public abstract class Fill
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | / |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | يحصل على رمز التجزئة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
            // تعيين نوع التعبئة إلى صلب وتعديل اللون
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = Color.LightBlue;

            Shape oval = worksheet.Shapes.AddOval(2, 0, 0, 0, 100, 150);
            // استخدام طريقة تعبئة التدرج مباشرةً على FillFormat
            oval.Fill.SetTwoColorGradient(Color.DarkBlue, Color.SkyBlue, GradientStyleType.Vertical, 0);

            workbook.Save("DrawingClassFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


