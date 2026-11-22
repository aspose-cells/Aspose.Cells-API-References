---
title: "ListObject.UpdateColumnName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListObject. تُحدّث أسماء جميع أعمدة القائمة إلى الخلايا في الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

يحدّث أسماء جميع أعمدة القائمة إلى الخلايا في الجدول.

```csharp
public void UpdateColumnName()
```

### ملاحظات

يجب أن تكون قيمة الخلايا في صف الرأس للجدول هي نفسها اسم ListColumn؛ لا تقوم Cell.PutValue بتعديل اسم ListColumn تلقائيًا لأداء أفضل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // إنشاء كائن جدول/قائمة
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // ملء بعض البيانات في الجدول
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // تحديث أسماء الأعمدة (سيتم تعيين أسماء افتراضية مثل Column1، Column2 إلخ.)
            listObject.UpdateColumnName();

            // احفظ المصنف
            wb.Save("output.xlsx");

            // تحقق من أن اسم العمود تم تحديثه
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


