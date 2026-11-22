---
title: "XmlMapCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة XmlMapCollection. أضف XmlMap باستخدام عنوان URL/مسار ملف xml/xsd"
type: docs
url: /ar/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

أضف [`XmlMap`](../../xmlmap/) عن طريق عنوان URL/المسار لملف xml/xsd.

```csharp
public int Add(string url)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| url | String | عنوان URL/المسار لملف xml/xsd. |

### قيمة الإرجاع

[`XmlMap`](../../xmlmap/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // أضف خرائط XML باستخدام المخطط وملفات XML
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


