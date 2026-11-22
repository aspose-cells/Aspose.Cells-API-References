---
title: "PivotTable.ShowReportFilterPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. إظهار جميع صفحات مرشح التقرير وفقًا لـ PivotField؛ يجب أن يكون PivotField موجودًا في PageFields"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

اعرض جميع صفحات مرشح التقرير وفقًا لـ PivotField، يجب أن يكون PivotField موجودًا في PageFields.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pageField | PivotField | كائن PivotField |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("source.xlsx");
            
            // الوصول إلى ورقة العمل الأولى وجدول محوري
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // عرض صفحات مرشح التقرير لكل حقل صفحة
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


