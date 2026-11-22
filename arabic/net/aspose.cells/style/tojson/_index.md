---
title: "Style.ToJson"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تحويل Style إلى بيانات هيكل JSON"
type: docs
url: /ar/net/aspose.cells/style/tojson/
---
## Style.ToJson method

تحويل [`Style`](../) إلى بيانات هيكل JSON.

```csharp
public string ToJson()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء وتطبيق نمط على الخلية B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // تحويل النمط إلى JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // حدد الصيغة في الخلية B6
            cells["B6"].Formula = "=A1";

            // تحويل الخلية إلى JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


