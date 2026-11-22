---
title: "Worksheet.AddPageBreaks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تضيف فاصل صفحة"
type: docs
url: /ar/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

يضيف فاصل صفحة.

```csharp
public void AddPageBreaks(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة فاصل صفحة أفقي عند الصف 1 (B2)
            worksheet.AddPageBreaks("B2");

            // إضافة فاصل صفحة أفقي عند الصف 9 (B10)
            worksheet.AddPageBreaks("B10");

            // تحقق من أن فاصل الصفحة الأول تم إضافته عند الصف 1
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


