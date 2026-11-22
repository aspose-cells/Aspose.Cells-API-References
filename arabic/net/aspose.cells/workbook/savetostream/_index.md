---
title: "Workbook.SaveToStream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحفظ ملف Excel إلى كائن MemoryStream كملف Excel972003 xls وتعيده"
type: docs
url: /ar/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

يحفظ ملف Excel إلى كائن MemoryStream كملف Excel97-2003 xls ويعيده.

```csharp
public MemoryStream SaveToStream()
```

### قيمة الإرجاع

كائن MemoryStream الذي يحتوي على ملف Excel بامتداد xls.

### ملاحظات

هذه الطريقة توفر نفس وظيفة طريقة Save وتقوم بحفظ دفتر العمل فقط كملف Excel97-2003 xls. تُستخدم أساسًا للاتصال من عملاء COM.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook start = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بعض البيانات النموذجية
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // حفظ دفتر العمل إلى تدفق الذاكرة
            MemoryStream stream = start.SaveToStream();

            // إنشاء دفتر عمل جديد من التدفق
            Workbook workbook = new Workbook(stream);

            // تعديل دفتر العمل الجديد
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // احفظ المصنف المعدل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


