---
title: "SaveOptions.WarningCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تحصل أو تعين رد الاتصال للتحذير"
type: docs
url: /ar/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

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
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // إنشاء خيارات الحفظ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين رد اتصال تحذير مخصص
            saveOptions.WarningCallback = new CustomWarningCallback();

            // سيؤدي هذا إلى توليد تحذير حول ميزة غير مدعومة في تنسيق HTML
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // حفظ مع خيارات قد تُحدث تحذيرات
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // معالجة التحذير - في هذه الحالة فقط عرضه
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### انظر أيضًا

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


