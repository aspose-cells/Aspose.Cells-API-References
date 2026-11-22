---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. True تعني أن الملف يحتوي على عدة ترميزات"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True يعني أن الملف يحتوي على عدة ترميزات.

```csharp
public bool IsMultiEncoded { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل النص
            TxtLoadOptions options = new TxtLoadOptions();
            
            // عيّن IsMultiEncoded إلى true لمعالجة الترميزات المتعددة
            options.IsMultiEncoded = true;
            
            // حمّل دفتر العمل باستخدام الخيارات
            Workbook workbook = new Workbook("example.csv", options);
            
            // اعرض قيمًا نموذجية من الملف المحمَّل
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


