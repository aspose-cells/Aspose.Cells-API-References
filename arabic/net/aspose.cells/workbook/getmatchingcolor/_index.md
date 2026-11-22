---
title: "Workbook.GetMatchingColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. العثور على اللون الأكثر تطابقًا في اللوحة الحالية"
type: docs
url: /ar/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

ابحث عن أفضل لون مطابق في لوحة الألوان الحالية.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rawColor | اللون | لون خام. |

### قيمة الإرجاع

أفضل لون مطابق.

### ملاحظات

هناك فقط 56 لونًا في لوحة ألوان Excel 97-2003. إذا لم يكن اللون موجودًا في اللوحة، سيتم تعيين لون مشابه.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // التحقق مما إذا كان اللون موجودًا في اللوحة
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // احصل على اللون المطابق من لوحة الألوان
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // إنشاء سمة مخصصة
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // الحصول على لون السمة
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


