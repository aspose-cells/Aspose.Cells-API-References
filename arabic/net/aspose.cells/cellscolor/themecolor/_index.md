---
title: "CellsColor.ThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. يحصل على لون السمة. ينطبق فقط على نوع لون السمة"
type: docs
url: /ar/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

يحصل على لون السمة. ينطبق فقط على نوع لون السمة.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorPropertyThemeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء مثال CellsColor
                CellsColor cellsColor = workbook.CreateCellsColor();

                // تعيين لون سمة
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // عرض خصائص ThemeColor
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // تطبيق اللون على خلية
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // احفظ المصنف
                workbook.Save("ThemeColorDemo.xlsx");
                Console.WriteLine("ThemeColor has been demonstrated successfully.");
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

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


