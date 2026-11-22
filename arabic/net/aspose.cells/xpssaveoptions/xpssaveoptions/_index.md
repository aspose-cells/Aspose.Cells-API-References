---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ XpsSaveOptions. ينشئ خيارات لحفظ ملف xps"
type: docs
url: /ar/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

إنشاء خيارات لحفظ ملف xps.

```csharp
public XpsSaveOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // تهيئة XpsSaveOptions باستخدام المنشئ
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // تكوين خيارات الحفظ
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // حفظ دفتر العمل باستخدام الخيارات
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

إنشاء خيارات لحفظ ملف xps.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | SaveFormat | تنسيق الحفظ، يجب أن يكون بتنسيق xps. |

### ملاحظات

ملاحظة: هذا المُنشئ أصبح الآن قديمًا. بدلاً من ذلك، يرجى استخدام مُنشئ XpsSaveOptions(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // إنشاء XpsSaveOptions باستخدام المُنشئ مع معامل SaveFormat
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // احفظ المصنف باستخدام الخيارات المحددة
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


