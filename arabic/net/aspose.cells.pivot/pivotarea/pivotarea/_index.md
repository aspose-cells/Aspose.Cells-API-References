---
title: "PivotArea.PivotArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ PivotArea. يعرض المنطقة المحددة من PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

يعرض المنطقة المحددة ل PivotTable.

```csharp
public PivotArea(PivotTable table)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الجدول | PivotTable |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // عرض مثال على منشئ PivotArea مع معامل PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // تكوين منطقة Pivot
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // احفظ المصنف
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


