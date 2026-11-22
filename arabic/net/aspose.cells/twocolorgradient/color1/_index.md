---
title: "TwoColorGradient.Color1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TwoColorGradient. يسترجع ويعيّن اللون الأول للتدرج"
type: docs
url: /ar/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

الحصول وتعيين لون التدرج الأول.

```csharp
public Color Color1 { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // إنشاء نمط مع تعبئة التدرج
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // تهيئة تدرج ثنائي اللون
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // تطبيق التدرج على نمط الخلية
            cell.SetStyle(style);
            
            // قراءة اللون الأولي
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // تعديل لون التدرج وإعادة تطبيقه
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // التحقق من التحديث
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // عرض بصري في ملف الإخراج
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


