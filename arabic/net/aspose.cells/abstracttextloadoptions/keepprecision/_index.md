---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractTextLoadOptions. تشير إلى عدم تحليل قيمة النص إذا كان طولها 15"
type: docs
url: /ar/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

يشير إلى عدم تحليل قيمة النص إذا كان طولها 15.

```csharp
public bool KeepPrecision { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML وتعيين KeepPrecision إلى true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // حمّل دفتر العمل باستخدام الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إظهار أن الدقة محفوظة (مثال: القيم الرقمية ذات الفواصل العشرية العديدة)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


