---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تتجاهل الصفوف/الأعمدة المخفية"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

يتجاهل الصفوف/الأعمدة المخفية.

```csharp
public bool IgnoreHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات عينة وتنسيق الصفوف
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // إخفاء الصف 1
            worksheet.Cells.Rows[1].IsHidden = true;

            // إنشاء AutoFitterOptions مع تعيين IgnoreHidden إلى true
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // ضبط الصفوف تلقائيًا مع تجاهل الصفوف المخفية
            worksheet.AutoFitRows(options);

            // إخراج ارتفاعات الصفوف
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


