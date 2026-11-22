---
title: "Cell.GetHtmlString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على سلسلة html التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية.

```csharp
public string GetHtmlString(bool html5)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| html5 | منطقي | يحدد ما إذا كانت القيمة متوافقة مع html5 |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين قيمة خلية عينة مع التنسيق
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // عرض GetHtmlString مع معامل منطقي
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


