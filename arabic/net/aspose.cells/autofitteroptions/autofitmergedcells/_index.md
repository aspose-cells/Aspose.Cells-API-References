---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تشير إلى ما إذا كان سيتم ضبط ارتفاع الصف تلقائيًا عندما يتم دمج الخلايا في صف. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

تشير إلى ما إذا كان سيتم ضبط ارتفاع الصف تلقائيًا عندما يتم دمج الخلايا في صف. القيمة الافتراضية هي false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية AutoFitterOptions.AutoFitMergedCellsType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات تجريبية ودمج الخلايا
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // إنشاء AutoFitterOptions وتعيين AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // ضبط تلقائي للصفوف مع خلايا مدمجة
            worksheet.AutoFitRows(options);

            // احفظ المصنف
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


