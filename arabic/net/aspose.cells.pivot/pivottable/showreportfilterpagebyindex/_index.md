---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. إظهار جميع صفحات مرشح التقرير وفقًا لمؤشر الموضع في PageFields"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

اعرض جميع صفحات مرشح التقرير وفقًا لمؤشر الموقع في PageFields.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| posIndex | Int32 | مؤشر الموضع في PageFields |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // الوصول إلى ورقة العمل الأولى التي تحتوي على جدول المحور
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // إظهار صفحات مرشح التقرير حسب الفهرس (الموضع) لحقل الصفحة
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // احفظ المصنف
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


