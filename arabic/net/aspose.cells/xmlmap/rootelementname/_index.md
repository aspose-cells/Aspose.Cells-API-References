---
title: "XmlMap.RootElementName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlMap. تحصل على اسم العنصر الجذر"
type: docs
url: /ar/net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

تحصل على اسم العنصر الجذر.

```csharp
public string RootElementName { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyRootElementNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بيانات تجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // إنشاء خريطة XML
            string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
            
            // احصل على اسم العنصر الجذر وعرضه
            string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
            Console.WriteLine("Root Element Name: " + rootElementName);
        }
    }
}
```

### انظر أيضًا

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


