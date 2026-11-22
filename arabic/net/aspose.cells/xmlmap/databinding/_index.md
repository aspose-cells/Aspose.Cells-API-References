---
title: "XmlMap.DataBinding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlMap. تحصل على XmlDataBinding لهذه الخريطة"
type: docs
url: /ar/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

تحصل على [`XmlDataBinding`](../../xmldatabinding/) لهذه الخريطة.

```csharp
public XmlDataBinding DataBinding { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف خرائط XML نموذجية
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // أضف خريطة XML الأولى
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // أضف خريطة XML الثانية
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // عرض استخدام خاصية DataBinding
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // احفظ المصنف
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


