---
title: "ReferredArea.StartRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. الصف الأول للمنطقة"
type: docs
url: /ar/net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

صف البداية للمنطقة.

```csharp
public int StartRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartRowDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وورقة عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // إنشاء نطاق مسمى يشير إلى A2:A4
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$2:$A$4";

            // احصل على المنطقة المشار إليها مع معامل إعادة الحساب
            ReferredArea area = name.GetReferredAreas(false)[0];

            // عرض خاصية StartRow
            Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
            Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
            Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3

            // التكرار عبر المنطقة المشار إليها باستخدام StartRow و EndRow
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
                Console.WriteLine("Value at row " + row + ": " + cell.Value);
            }
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


