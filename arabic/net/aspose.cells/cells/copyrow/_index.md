---
title: "Cells.CopyRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تنسخ البيانات والتنسيقات لصف كامل"
type: docs
url: /ar/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

ينسخ البيانات والتنسيقات لصف كامل.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | Int32 | فهرس الصف المصدر. |
| destinationRowIndex | Int32 | فهرس الصف الوجهة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // أضف بعض البيانات إلى الصف الأول
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // إنشاء ورقة عمل ثانية
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // نسخ الصف من Sheet1 إلى Sheet2
            cells2.CopyRow(cells1, 0, 0);
            
            // نسخ الصف داخل Sheet1 إلى مواضع جديدة
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // احفظ المصنف
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


