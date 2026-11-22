---
title: "ThemeColor.ThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ ThemeColor."
type: docs
url: /ar/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ThemeColorType | نوع السمة. |
| ظل | Double | قيمة الظل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // استدعاء طريقة #ctor مع معلمات ThemeColorType و Double
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // تطبيق لون السمة على نمط الخلية
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


