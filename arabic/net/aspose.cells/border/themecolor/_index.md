---
title: "Border.ThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Border. يحصل ويضبط لون السمة للحد"
type: docs
url: /ar/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

يحصل ويضبط لون السمة للحد.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى خلية والحصول على نمطها
            Style style = worksheet.Cells["A1"].GetStyle();

            // ضبط لون سمة الحد
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // تطبيق النمط على الخلية
            worksheet.Cells["A1"].SetStyle(style);

            // احفظ المصنف
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


