---
title: "FindOptions.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. الصيغة المراد البحث عنها"
type: docs
url: /ar/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

الصيغة المراد البحث عنها.

```csharp
public Style Style { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ نمطًا بخط أزرق
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // طبق النمط على الخلية F2
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // أنشئ خيارات البحث مع النمط
            FindOptions options = new FindOptions();
            options.Style = style;

            // ابحث عن خلية ذات نمط مطابق
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // أخرج اسم الخلية التي تم العثور عليها
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


