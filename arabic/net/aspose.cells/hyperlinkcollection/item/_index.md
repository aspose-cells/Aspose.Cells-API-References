---
title: "HyperlinkCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HyperlinkCollection. تحصل على عنصر Hyperlink عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

يحصل على عنصر [`Hyperlink`](../../hyperlink/) عند الفهرس المحدد.

```csharp
public Hyperlink this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط تشعبي إلى الخلية A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // الوصول إلى أول ارتباط تشعبي باستخدام خاصية Item وتعيين نص العرض
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // تعيين نمط الارتباط التشعبي (نص أزرق تحته خط)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


