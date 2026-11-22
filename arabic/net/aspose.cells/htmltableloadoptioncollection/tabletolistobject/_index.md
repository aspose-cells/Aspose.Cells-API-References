---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlTableLoadOptionCollection. تشير إلى ما إذا كان يتم إنشاء كائنات قائمة من الجداول المستوردة. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

يشير إلى ما إذا كان سيتم إنشاء كائنات قائمة من الجداول المستوردة. القيمة الافتراضية هي false.

```csharp
public bool TableToListObject { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // الوصول إلى مثال HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // قم بتعيين خاصية TableToListObject لتحويل جداول HTML إلى ListObjects
            tableLoadOptions.TableToListObject = true;

            // أضف جدولًا ليتم تحويله إلى ListObject حسب الفهرس
            tableLoadOptions.Add(0);

            // تحميل ملف HTML إلى المصنف باستخدام خيارات التحميل
            workbook = new Workbook("input.html", loadOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


