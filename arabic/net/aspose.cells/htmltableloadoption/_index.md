---
title: "الفئة HtmlTableLoadOption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.HtmlTableLoadOption. تمثل الخيار عند استيراد جدول من HTML"
type: docs
url: /ar/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

يمثل الخيار عند استيراد جدول من HTML.

```csharp
public class HtmlTableLoadOption
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | احصل أو عيّن معرف الجدول لاستيراده من HTML |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) احصل أو عيّن اسم الجدول لاستيراده من HTML |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | احصل أو عيّن الفهرس الأصلي لورقة العمل في HTML. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | احصل أو عيّن فهرس الجدول لاستيراده من HTML. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | يشير إلى ما إذا كان سيتم إنشاء كائنات قائمة من الجدول المستورد. القيمة الافتراضية هي false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | احصل أو عيّن الفهرس الهدف لورقة العمل حيث سيتم وضع الجدول. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // أنشئ مثيلًا من HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // إنشاء نسخة من HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // إضافة HtmlTableLoadOption إلى HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // تحميل ملف HTML إلى المصنف باستخدام خيارات التحميل المحددة
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


