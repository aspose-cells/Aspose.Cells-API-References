---
title: "LoadOptions.AutoFitterOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل وتعيّن خيارات الضبط التلقائي"
type: docs
url: /ar/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

يحصل ويضبط خيارات الملاءمة التلقائية

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### ملاحظات

فقط لملفات xlsx ، spreadsheetML الآن.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // إنشاء AutoFitterOptions وتعيين الخصائص
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // إنشاء LoadOptions وتعيين AutoFitterOptions
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // تحميل دفتر العمل باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // إظهار الضبط التلقائي بالحصول على ارتفاع الصف
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


