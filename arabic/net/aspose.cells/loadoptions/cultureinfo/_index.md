---
title: "LoadOptions.CultureInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعين الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله"
type: docs
url: /ar/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### ملاحظات

هذه الخاصية لها نفس التأثير مع [`Region`](../region/) لتعيين الإعدادات الإقليمية.

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // إنشاء ملف Excel تجريبي
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // التحميل مع ثقافة محددة
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


