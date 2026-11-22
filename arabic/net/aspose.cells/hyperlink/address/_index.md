---
title: "Hyperlink.Address"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Hyperlink. تمثل عنوان الارتباط التشعبي"
type: docs
url: /ar/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

يمثل عنوان الارتباط التشعبي.

```csharp
public string Address { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف روابط تشعبية بعناوين مختلفة
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // الوصول إلى عناوين الروابط التشعبية وعرضها
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // احفظ المصنف
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


