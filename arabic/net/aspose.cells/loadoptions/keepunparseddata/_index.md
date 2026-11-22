---
title: "LoadOptions.KeepUnparsedData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. ما إذا كان يجب الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

ما إذا كان سيتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عندما يتم تحميله من ملف القالب. القيمة الافتراضية هي true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### ملاحظات

للحالات التي يحتاج فيها المستخدم فقط إلى قراءة بعض المحتويات من ملف القالب ولا يحتاج إلى حفظ المصنف مرة أخرى، قد يؤدي ضبط هذه الخاصية على false إلى تحسين الأداء، خاصةً عند استخدامها مع نوع من LoadFilter،

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل وضبط KeepUnparsedData إلى false
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // تحميل دفتر العمل مع الخيارات
            Workbook workbook = new Workbook("example.xlsx", options);

            // الوصول إلى ورقة العمل وإظهار أن البيانات غير المُحلَّلة غير محفوظة
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


