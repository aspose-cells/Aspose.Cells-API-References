---
title: "Border.ArgbColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Border. يحصل على أو يضبط اللون باستخدام قيمة ARGB 32‑بت"
type: docs
url: /ar/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

يحصل ويضبط اللون باستخدام قيمة ARGB ذات 32 بت.

```csharp
public int ArgbColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية B2 وضبط قيمة
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // احصل على النمط والحدود
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // ضبط خصائص الحد بما في ذلك لون ARGB
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // تطبيق النمط المعدل على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("BorderArgbColorDemo.xlsx");

            // تحقق من أن لون ARGB تم ضبطه بشكل صحيح
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### انظر أيضًا

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


