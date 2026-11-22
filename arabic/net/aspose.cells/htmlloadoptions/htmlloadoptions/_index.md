---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ HtmlLoadOptions. ينشئ خيارات لتحميل الملف"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

إنشاء خيارات تحميل الملف.

```csharp
public HtmlLoadOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML باستخدام المنشئ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // تحميل ملف HTML باستخدام الخيارات
            Workbook workbook = new Workbook("example.html", loadOptions);

            // الوصول إلى البيانات من HTML المحمّل
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

إنشاء خيارات تحميل الملف.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | LoadFormat | صيغة التحميل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء كائن HtmlLoadOptions باستخدام المنشئ مع معامل LoadFormat
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // تعيين بعض خصائص HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // إنشاء دفتر عمل باستخدام خيارات التحميل
                Workbook workbook = new Workbook("input.html", loadOptions);

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض بعض المعلومات حول HTML المحمل
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // احفظ المصنف
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


