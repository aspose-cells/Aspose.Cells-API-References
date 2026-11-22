---
title: "Cells.MaxDataRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. أقصى فهرس صف للخلية التي تحتوي على بيانات"
type: docs
url: /ar/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات.

```csharp
public int MaxDataRow { get; }
```

### ملاحظات

إرجاع -1 إذا لم توجد خلية تحتوي على بيانات. تحتاج هذه الخاصية إلى تكرار وفحص الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرة كشرط في حلقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // عرض استخدام MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // إنشاء منطقة خلايا باستخدام MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // تطبيق التنسيق على نطاق البيانات
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // تطبيق النمط على النطاق
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // احفظ المصنف
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


