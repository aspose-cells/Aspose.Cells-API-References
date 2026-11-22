---
title: "Cells.MaxRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحد الأقصى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط"
type: docs
url: /ar/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط.

```csharp
public int MaxRow { get; }
```

### ملاحظات

إرجاع -1 إذا لم توجد خلية تحتوي على بيانات أو نمط في ورقة العمل. تحتاج هذه الخاصية إلى التكرار وفحص الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية مستهلكة للوقت ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بعض البيانات التجريبية
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // احصل على مؤشر الصف الأقصى (بدءًا من الصفر)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // أضف بيانات جديدة في الصف التالي بعد الصف الأقصى
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // تحقق من الصف الأقصى الجديد
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // احفظ المصنف
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


