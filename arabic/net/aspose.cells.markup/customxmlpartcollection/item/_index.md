---
title: "CustomXmlPartCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomXmlPartCollection. تحصل على عنصر بالمؤشر المحدد"
type: docs
url: /ar/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

يحصل على عنصر في الفهرس المحدد.

```csharp
public CustomXmlPart this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى CustomXmlPartCollection مباشرةً من المصنف
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // بيانات XML نموذجية
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // إضافة جزء XML مخصص
            int index = customXmlParts.Add(xmlBytes, null);
            
            // الوصول إلى العنصر باستخدام خاصية Item
            CustomXmlPart part = customXmlParts[index];
            
            // عرض معرف الجزء XML المخصص
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // استرجاع بيانات XML من الجزء
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // احفظ المصنف
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


