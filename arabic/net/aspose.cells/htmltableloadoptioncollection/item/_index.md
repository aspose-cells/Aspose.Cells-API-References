---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlTableLoadOptionCollection. تحصل على عنصر HtmlTableLoadOption في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

يحصل على عنصر [`HtmlTableLoadOption`](../../htmltableloadoption/) في الفهرس المحدد.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // إضافة HtmlTableLoadOption جديد حسب فهرس الجدول
            int index1 = tableLoadOptions.Add(0);

            // الوصول إلى HtmlTableLoadOption باستخدام خاصية Item
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // تكوين خيار تحميل الجدول
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // تحميل ملف HTML مع الخيارات المكوّنة
            Workbook workbook = new Workbook("input.html", loadOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


