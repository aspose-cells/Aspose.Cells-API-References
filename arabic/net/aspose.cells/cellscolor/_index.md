---
title: "الفئة CellsColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellsColor. تمثل جميع أنواع اللون"
type: docs
url: /ar/net/aspose.cells/cellscolor/
---
## CellsColor class

يمثل جميع أنواع اللون.

```csharp
public class CellsColor
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | يحصل على اللون ويضبطه من قيمة ARGB 32-بت. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | يحصل على اللون RGB ويضبطه. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | يحصل على فهرس اللون في لوحة الألوان ويضبطه. ينطبق فقط على اللون المفهرس. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | يحصل على اللون ويضبطه الذي يجب تطبيقه على الخلية أو الشكل. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | يحصل على لون السمة. ينطبق فقط على نوع لون السمة. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | يحصل على الشفافية ويضبطها كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | نوع اللون. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | ضبط درجة لون الشكل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق من الخلايا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // إنشاء مثال CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // ضبط خصائص CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // تطبيق CellsColor على النطاق
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // احفظ المصنف
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


