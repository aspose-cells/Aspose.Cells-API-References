---
title: "Hyperlink.ScreenTip"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Hyperlink. تُرجع أو تعيّن نص ScreenTip للارتباط التشعبي المحدد"
type: docs
url: /ar/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

إرجاع أو تعيين نص تلميح الشاشة للرابط التشعبي المحدد.

```csharp
public string ScreenTip { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // إنشاء ارتباط تشعبي مع ScreenTip
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // احفظ المصنف
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


