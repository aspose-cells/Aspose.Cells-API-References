---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. يحصل على فواصل الصفحات الأفقية لهذا جدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

يحصل على فواصل الصفحات الأفقية لهذا جدول المحور.

```csharp
public int[] GetHorizontalPageBreaks()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف المصدر
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تحديث وحساب بيانات جدول البيفوت
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احصل على فواصل الصفحات الأفقية
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // عرض النتائج
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


