---
title: "ThemeColor.Tint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThemeColor. تحصل وتضبط قيمة الظل"
type: docs
url: /ar/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

يحصل ويضبط قيمة التدرج.

```csharp
public double Tint { get; set; }
```

### ملاحظات

قيمة الظل تُخزن كعدد مزدوج من -1.0 إلى 1.0، حيث -1.0 يعني تعتيم بنسبة 100% و1.0 يعني إضاءة بنسبة 100%. أيضًا، 0.0 يعني عدم تغيير.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط بلون السمة والظل
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // احصل على قيمة الظل من نمط الخلية
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // تعديل قيمة الظل
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // تحقق من قيمة الظل الجديدة
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### انظر أيضًا

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


