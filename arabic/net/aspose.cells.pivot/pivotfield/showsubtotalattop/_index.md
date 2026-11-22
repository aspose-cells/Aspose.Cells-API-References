---
title: "PivotField.ShowSubtotalAtTop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر.

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### ملاحظات

يعمل فقط مع الحقول المحورية في منطقة الصف عندما تكون ShowInOutlineForm صحيحة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowSubtotalAtTopDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B5"].Value = 2500;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // إضافة حقل صف وتكوين موضع المجموع الفرعي
            PivotField rowField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, "Product")];
            rowField.ShowSubtotalAtTop = true; // Demonstrate the property
            rowField.IsAutoSubtotals = true;

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احفظ المصنف
            workbook.Save("PivotFieldShowSubtotalAtTopDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


