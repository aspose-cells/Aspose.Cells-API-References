---
title: "الفئة ThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ThemeColor. يمثل لونًا من السمة"
type: docs
url: /ar/net/aspose.cells/themecolor/
---
## ThemeColor class

يمثل لونًا للثيم.

```csharp
public class ThemeColor
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | يحصل ويضبط نوع السمة. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | يحصل ويضبط قيمة التدرج. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // إضافة قيمة إلى الخلية A1
            cells["A1"].PutValue("Hello World");

            // الحصول على نمط الخلية A1
            Style style = cells["A1"].GetStyle();

            // تعيين نوع اللون ThemeColorType.Text2 بإنارة 40% كلون الخط.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // تعيين نوع اللون ThemeColorType.Background2 بتغميق 75% كلون المقدمة.
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // تطبيق النمط على الخلية A1
            cells["A1"].SetStyle(style);

            // حفظ ملف Excel
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


