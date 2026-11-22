---
title: "Worksheet.PivotTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تسترجع جميع جداول المحور في هذه الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

يحصل على جميع جداول المحور في هذه ورقة العمل.

```csharp
public PivotTableCollection PivotTables { get; }
```

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة جداول المحور من worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // تحقق مما إذا كان هناك أي جداول محور
            if (pivotTables.Count > 0)
            {
                // احصل على أول جدول محور
                PivotTable pivotTable = pivotTables[0];
                
                // مسح أي عوامل تصفية موجودة
                pivotTable.PivotFilters.Clear();
                
                // تحديث بيانات جدول المحور
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // احفظ المصنف المعدل
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


