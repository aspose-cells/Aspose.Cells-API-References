---
title: "Cells.GetLastDataRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على فهرس الصف الأخير للخلية التي تحتوي على بيانات في العمود المحدد"
type: docs
url: /ar/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

يحصل على فهرس الصف الأخير للخلية التي تحتوي على بيانات في العمود المحدد.

```csharp
public int GetLastDataRow(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

فهرس الصف الأخير.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // احصل على الصف البيانات الأخير في العمود A (الفهرس 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // أخرج النتيجة.
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // إدراج صف جديد بعد الصف البيانات الأخير
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // إضافة بيانات إلى الصف الجديد
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


