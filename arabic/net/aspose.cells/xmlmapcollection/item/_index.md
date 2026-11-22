---
title: "XmlMapCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlMapCollection. تحصل على خريطة xml حسب الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

يحصل على خريطة XML وفق الفهرس المحدد.

```csharp
public XmlMap this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

خريطة xml

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى XmlMapCollection من المصنف
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // أضف XmlMap جديد إلى المجموعة
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // الوصول إلى XmlMap باستخدام خاصية Item
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // عرض اسم XmlMap
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // احفظ المصنف
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


