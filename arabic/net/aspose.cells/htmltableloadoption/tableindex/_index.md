---
title: "HtmlTableLoadOption.TableIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlTableLoadOption. احصل أو عيّن فهرس الجدول لاستيراده من html"
type: docs
url: /ar/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

احصل أو عيّن فهرس الجدول لاستيراده من HTML.

```csharp
public int TableIndex { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // تكوين خيار تحميل الجدول مع TableIndex = 0 (الجدول الأول)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // إضافة خيار تحميل الجدول
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // تحميل ملف HTML (استبدل بالمسار الفعلي)
            workbook = new Workbook("input.html", loadOptions);

            // حفظ كملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


