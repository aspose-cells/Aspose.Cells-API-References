---
title: "PivotTable.DisplayNullString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/displaynullstring/
---
## PivotTable.DisplayNullString property

يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة.

```csharp
public bool DisplayNullString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayNullStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue(null);
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(null);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // تعيين خاصية DisplayNullString وسلسلة فارغة مخصصة
            pivotTable.DisplayNullString = true;
            pivotTable.NullString = "N/A";
            
            // حساب البيانات وتحديث الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableDisplayNullStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


