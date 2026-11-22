---
title: "AutoFitterOptions.FormatStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تحصل وتعيين استراتيجية التنسيق"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

يحصل ويضبط الاستراتيجية المُنسقة.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### ملاحظات

القيمة الافتراضية هي CellStyle للأداء.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات تجريبية وتغليف النص
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // إنشاء AutoFitterOptions مع FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // تطبيق الضبط التلقائي باستخدام الخيارات المحددة
            worksheet.AutoFitRows(options);

            // حفظ النتيجة
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


