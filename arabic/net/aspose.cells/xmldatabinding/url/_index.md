---
title: "XmlDataBinding.Url"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlDataBinding. تحصل على عنوان URL المصدر لهذا ربط البيانات"
type: docs
url: /ar/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

يحصل على عنوان url المصدر لهذا الربط البيانات.

```csharp
public string Url { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class XmlDataBindingPropertyUrlDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقتي عمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // إضافة كائنات القائمة وخرائط XML
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // الحصول على عناوين URL لربط بيانات XML (Url للقراءة فقط)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // عرض عناوين URL
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // احفظ المصنف
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


