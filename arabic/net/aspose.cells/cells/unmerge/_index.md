---
title: "Cells.UnMerge"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تلغي دمج نطاق محدد من الخلايا المدمجة"
type: docs
url: /ar/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

يفك دمج نطاق محدد من الخلايا المدمجة.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من هذا النطاق (مؤشر صفر) |
| firstColumn | Int32 | العمود الأول من هذا النطاق (مؤشر صفر) |
| totalRows | Int32 | عدد الصفوف (مؤشر واحد) |
| totalColumns | Int32 | عدد الأعمدة (مؤشر واحد) |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ادمج الخلايا أولاً
            cells.Merge(0, 0, 2, 2);
            
            // إلغاء دمج الخلايا المدمجة مسبقاً
            cells.UnMerge(0, 0, 2, 2);
            
            // احفظ المصنف
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


