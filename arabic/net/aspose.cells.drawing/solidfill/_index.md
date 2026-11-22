---
title: "الفئة SolidFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.SolidFill. تغلف الكائن الذي يمثل تنسيق التعبئة الصلبة"
type: docs
url: /ar/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

يغلف الكائن الذي يمثل تنسيق التعبئة الصلبة

```csharp
public class SolidFill : Fill
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | يحصل على كائن [`CellsColor`](./cellscolor/) ويضبطه. |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | يحصل على اللون أو يضبطه. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | يحصل على رمز التجزئة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // أضف شكل مستطيل بسيط إلى الورقة
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // قم بتكوين الشكل لاستخدام تعبئة صلبة
                rect.Fill.FillType = FillType.Solid;

                // احصل على كائن SolidFill
                SolidFill solidFill = rect.Fill.SolidFill;

                // ضبط خصائص التعبئة الصلبة
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // الوصول إلى خاصية CellsColor (قراءة/كتابة)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // احفظ المصنف للتحقق من مظهر الشكل
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


