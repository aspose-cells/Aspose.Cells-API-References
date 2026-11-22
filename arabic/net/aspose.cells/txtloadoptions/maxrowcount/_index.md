---
title: "TxtLoadOptions.MaxRowCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. الحد الأقصى لعدد الصفوف التي سيتم استيرادها لورقة واحدة"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

الحد الأقصى لعدد الصفوف التي سيتم استيرادها لورقة واحدة.

```csharp
public int MaxRowCount { get; set; }
```

### ملاحظات

الصفوف التي تتجاوز هذا الحد سيتم تجاهلها أو تمديدها إلى الورقة التالية وفقًا لـ [`ExtendToNextSheet`](../extendtonextsheet/). هذا العدد يشمل صفوف الرأس ([`HeaderRowsCount`](../headerrowscount/)). القيمة القصوى المسموح بها هي حد الصفوف لتنسيق الملف المقابل، مثل ملف xlsx حيث يكون 1048576. إذا لم يتم تحديد هذه الخاصية أو كانت القيمة المحددة غير موجبة، فسيتم استخدام الحد الأقصى أيضًا.

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // إنشاء محتوى CSV نموذجي
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // إنشاء TxtLoadOptions مع تعيين MaxRowCount إلى 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // تحميل ملف CSV إلى دفتر العمل
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // تحقق من أنه تم تحميل 4 صفوف فقط (صف رأس واحد + 3 صفوف بيانات)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // سيكون هذا فارغًا لأننا قمنا بتحميل 4 صفوف فقط (الفهرس 0-3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


