---
title: "Hyperlink.Area"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Hyperlink. تحصل على نطاق الارتباط التشعبي"
type: docs
url: /ar/net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

يحصل على نطاق الارتباط التشعبي.

```csharp
public CellArea Area { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Main Menu");
            worksheet.Cells["A3"].PutValue("Chapter 1");
            worksheet.Cells["A4"].PutValue("Chapter 2");
            
            // أضف روابط تشعبية
            int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
            int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");

            // الوصول إلى الروابط التشعبية وإظهار استخدام خاصية Area
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            string chapter2Address = "";
            foreach (Hyperlink link in hyperlinks)
            {
                // تحقق مما إذا كان الارتباط التشعبي في الخلية A4 باستخدام خاصية Area
                if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
                {
                    chapter2Address = link.Address;
                    break;
                }
            }

            Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


