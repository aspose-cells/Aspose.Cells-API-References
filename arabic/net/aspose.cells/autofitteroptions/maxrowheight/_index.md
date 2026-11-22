---
title: "AutoFitterOptions.MaxRowHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تحصل وتعيين أقصى ارتفاع للصف بوحدة النقطة عند ضبط الصفوف تلقائيًا"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

يحصل ويضبط الحد الأقصى لارتفاع الصف (بوحدة النقطة) عند ضبط الصفوف تلقائيًا.

```csharp
public double MaxRowHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyMaxRowHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات نموذجية وتنسيق
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row auto-fitting");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells.SetRowHeight(0, 10); // Set initial small row height

            // إنشاء AutoFitterOptions مع إعداد MaxRowHeight
            AutoFitterOptions options = new AutoFitterOptions
            {
                MaxRowHeight = 50, // Limit maximum row height to 50 pixels
                OnlyAuto = true
            };

            // ضبط الصف تلقائيًا مع تحديد الحد الأعلى للارتفاع
            worksheet.AutoFitRows(0, 0, options);

            Console.WriteLine("Row height after auto-fit with MaxRowHeight=50: " + worksheet.Cells.GetRowHeight(0));

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


