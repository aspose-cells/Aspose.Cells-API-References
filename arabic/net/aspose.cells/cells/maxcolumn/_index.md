---
title: "Cells.MaxColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحد الأقصى لمؤشر العمود لتلك الخلايا التي تم إنشاءها في المجموعة لا يشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه"
type: docs
url: /ar/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

الحد الأقصى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له للعمود بأكمله ولكن لم يتم إنشاء أي خلية فيه).

```csharp
public int MaxColumn { get; }
```

### ملاحظات

أرجع -1 إذا لم يتم إنشاء أي خلية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // احصل على الحد الأقصى لمؤشر العمود الذي يحتوي على بيانات
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // أضف بيانات إلى العمود التالي بعد العمود الأقصى
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // تحقق من العمود الأقصى الجديد
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // أنشئ ورقة عمل أخرى لتوضيح النسخ
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // انسخ جميع الأعمدة من المصدر إلى الوجهة
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


