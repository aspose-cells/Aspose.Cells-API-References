---
title: "LoadOptions.WarningCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعين رد النداء التحذيري"
type: docs
url: /ar/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

يحصل أو يضبط رد النداء التحذيري.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // إنشاء رد نداء تحذيري مخصص
            IWarningCallback warningCallback = new CustomWarningCallback();

            // تهيئة خيارات التحميل مع رد النداء التحذيري
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // تحميل دفتر العمل مع الخيارات
            Workbook workbook = new Workbook("example.xlsx", options);

            // إظهار استخدام رد النداء التحذيري عن طريق الوصول إلى خلية
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


