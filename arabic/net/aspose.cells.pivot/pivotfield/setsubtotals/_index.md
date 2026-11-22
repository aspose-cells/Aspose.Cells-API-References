---
title: "PivotField.SetSubtotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تحدد كيفية حساب الإجماليات الفرعية للحقل المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

يحدد كيفية تجميع المجموع الفرعي للحقل المحدد.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | [`PivotFieldSubtotalType`](../../pivotfieldsubtotaltype/) |
| معروض | منطقي | ما إذا كان الحقل المحدد يظهر تلك الإجماليات الفرعية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            var cells = sheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = "TV";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Electronics";
            cells["B3"].Value = "Radio";
            cells["C3"].Value = 500;
            
            cells["A4"].Value = "Clothing";
            cells["B4"].Value = "Shirt";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "Clothing";
            cells["B5"].Value = "Pants";
            cells["C5"].Value = 400;

            // إضافة جدول محوري
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // إضافة حقول الصف
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // عرض SetSubtotals باستخدام PivotFieldSubtotalType والقيمة المنطقية
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


