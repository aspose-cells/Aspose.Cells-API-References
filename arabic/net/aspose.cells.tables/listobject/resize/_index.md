---
title: "ListObject.Resize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListObject. تغيير حجم نطاق كائن القائمة"
type: docs
url: /ar/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

تغيير حجم النطاق لكائن القائمة.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي للنطاق الجديد. |
| startColumn | Int32 | فهرس العمود الابتدائي للنطاق الجديد. |
| endRow | Int32 | فهرس الصف النهائي للنطاق الجديد. |
| endColumn | Int32 | فهرس العمود النهائي للنطاق الجديد. |
| hasHeaders | منطقي | ما إذا كان هذا الجدول يحتوي على رؤوس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // تغيير حجم كائن القائمة
            listObj.Resize(0, 0, 9, 1, true);

            // احفظ المصنف
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


