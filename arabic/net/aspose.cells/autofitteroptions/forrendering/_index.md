---
title: "AutoFitterOptions.ForRendering"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تشير إلى ما إذا كان الملاءمة لغرض العرض"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

يوضح ما إذا كان مناسبًا لأغراض العرض.

```csharp
public bool ForRendering { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات عينة بنص طويل
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // إنشاء AutoFitterOptions وتعيين ForRendering إلى true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // ضبط تلقائي للصف مع مراعاة العرض
            worksheet.AutoFitRows(0, 0, options);

            // إخراج ارتفاع الصف الناتج بالبكسل
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


