---
title: "Spinner.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Spinner. تشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

يشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد.

```csharp
public bool Shadow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة Spinner إلى ورقة العمل.
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // اضبط خصائص Spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // عرض خاصية Shadow
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // احفظ المصنف
            workbook.Save("SpinnerShadowDemo.xlsx");

            // تحميل المصنف المحفوظ للتحقق من خاصية الظل
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


