---
title: "Cells.LastCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على الخلية الأخيرة في هذه ورقة العمل"
type: docs
url: /ar/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

يحصل على الخلية الأخيرة في ورقة العمل هذه.

```csharp
public Cell LastCell { get; }
```

### ملاحظات

يعيد null إذا لم توجد بيانات في ورقة العمل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // احصل على عنوان الخلية الأخيرة
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // إنشاء نطاق من الخلية الأولى إلى الأخيرة
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // تطبيق التنسيق على range
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // احفظ المصنف
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


