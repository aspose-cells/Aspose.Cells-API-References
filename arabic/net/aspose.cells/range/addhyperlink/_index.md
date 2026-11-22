---
title: "Range.AddHyperlink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تضيف ارتباطًا تشعبيًا إلى خلية محددة أو إلى نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| address | String | عنوان الارتباط التشعبي. |
| textToDisplay | String | النص الذي سيتم عرضه للارتباط التشعبي المحدد. |
| screenTip | String | نص الـ screenTip للارتباط التشعبي المحدد. |

### قيمة الإرجاع

[`Hyperlink`](../../hyperlink/) object.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // إضافة ارتباط تشعبي مع العنوان، النص المعروض وتلميح الشاشة
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // احفظ المصنف
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


