---
title: "Worksheet.Hyperlinks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على مجموعة HyperlinkCollection"
type: docs
url: /ar/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

يحصل على مجموعة [`HyperlinkCollection`](../../hyperlinkcollection/).

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف ارتباطًا تشعبيًا إلى ورقة العمل
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // احفظ المصنف
            workbook.Save("HyperlinksDemo.xlsx");
            
            // حمّل دفتر العمل المحفوظ للتحقق من الارتباط التشعبي
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // عرض عنوان الارتباط التشعبي
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### انظر أيضًا

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


