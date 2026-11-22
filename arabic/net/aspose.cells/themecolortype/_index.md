---
title: "تعداد ThemeColorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ThemeColorType. يعدد أنواع ألوان السمة"
type: docs
url: /ar/net/aspose.cells/themecolortype/
---
## ThemeColorType enumeration

يسرد أنواع ألوان السمة.

```csharp
public enum ThemeColorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Background1 | `0` |  |
| Text1 | `1` |  |
| Background2 | `2` |  |
| Text2 | `3` |  |
| Accent1 | `4` |  |
| Accent2 | `5` |  |
| Accent3 | `6` |  |
| Accent4 | `7` |  |
| Accent5 | `8` |  |
| Accent6 | `9` |  |
| Hyperlink | `10` |  |
| FollowedHyperlink | `11` |  |
| StyleColor | `12` | Inner مستخدم. لون يُستخدم في تعريفات السمة يعني استخدام لون النمط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassThemeColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // الوصول إلى الخلية A1 والحصول على نمطها
            Style style = cells["A1"].GetStyle();
            
            // تعيين نمط صلب بلون المقدمة الأحمر
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            
            // تعيين نمط gray12 بلون المقدمة الأزرق وخلفية صفراء
            style.Pattern = BackgroundType.Gray12;
            style.ForegroundColor = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            Console.WriteLine("Background ARGB Color: " + style.BackgroundArgbColor);
            
            // تعيين ألوان السمة
            ThemeColor foregroundTheme = new ThemeColor(ThemeColorType.Accent6, 0.5);
            ThemeColor backgroundTheme = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.ForegroundThemeColor = foregroundTheme;
            style.BackgroundThemeColor = backgroundTheme;
            
            Console.WriteLine("Foreground Theme Color Type: " + style.ForegroundThemeColor.ColorType);
            Console.WriteLine("Background Theme Color Type: " + style.BackgroundThemeColor.ColorType);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


