---
title: "ListColumn.Formula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListColumn. تحصل وتضبط الصيغة لعمود القائمة"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

يحصل على صيغة العمود في القائمة ويضبطها.

```csharp
public string Formula { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات تجريبية وجدول
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // إضافة صيغة إلى عمود القائمة
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // احفظ المصنف
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


