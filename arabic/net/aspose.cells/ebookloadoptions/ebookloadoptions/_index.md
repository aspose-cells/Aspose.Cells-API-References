---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ EbookLoadOptions. ينشئ خيارًا لتحميل ملف الكتاب الإلكتروني"
type: docs
url: /ar/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

ينشئ خيارًا لتحميل ملف الكتاب الإلكتروني.

```csharp
public EbookLoadOptions()
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // أنشئ مثيلًا من EbookLoadOptions باستخدام المنشئ
            EbookLoadOptions options = new EbookLoadOptions();

            // تعيين بعض الخصائص الأساسية
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // حمّل ملف كتاب إلكتروني باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("sample.epub", options);
            
            // حفظ كملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

ينشئ خيارًا لتحميل ملف الكتاب الإلكتروني.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | LoadFormat | تنسيق التحميل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مثيلًا من EbookLoadOptions مع معامل LoadFormat
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // اعرض التأكيد
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // مثال على الاستخدام: حمّل دفتر عمل بهذه الخيارات
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // حفظ النتيجة
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


