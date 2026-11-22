---
title: "HtmlTableLoadOption.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlTableLoadOption. احصل أو عيّن اسم الجدول لاستيراده من html"
type: docs
url: /ar/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

احصل أو عيّن اسم الجدول لاستيراده من html

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // الوصول إلى HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // إضافة HtmlTableLoadOption جديد حسب فهرس الجدول
            int index = tableLoadOptions.Add(0);

            // الوصول إلى HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // عيّن خاصية Name
            option.Name = "CustomerDataTable";

            // تحميل ملف HTML (استبدل بمسار الملف الفعلي)
            workbook = new Workbook("input.html", loadOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


