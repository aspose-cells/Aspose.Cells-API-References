---
title: "PivotTable.ShowDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. إظهار تفاصيل عنصر واحد في منطقة البيانات إلى جدول جديد"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

اعرض تفاصيل عنصر واحد في منطقة البيانات إلى جدول جديد.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | الإزاحة إلى الصف البيانات الأول في منطقة البيانات. |
| columnOffset | Int32 | الإزاحة إلى عمود البيانات الأول في منطقة البيانات. |
| newSheet | منطقي | إظهار التفاصيل إلى ورقة عمل جديدة. |
| destRow | Int32 | الصف المستهدف. |
| destColumn | Int32 | العمود المستهدف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // إظهار التفاصيل للخلية المحددة
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // احفظ المصنف
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


