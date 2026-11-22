---
title: "Cells.MinDataRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحد الأدنى لرقم الصف للخلية التي تحتوي على بيانات"
type: docs
url: /ar/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات.

```csharp
public int MinDataRow { get; }
```

### ملاحظات

إرجاع -1 إذا لم توجد خلية تحتوي على بيانات. تحتاج هذه الخاصية إلى تكرار وفحص الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرة كشرط في حلقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // عرض مثال لاستخدام MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // احفظ المصنف
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


