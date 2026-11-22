---
title: "PivotField.DragToPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/dragtopage/
---
## PivotField.DragToPage property

يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحات. القيمة الافتراضية هي true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToPage { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToPage. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToPageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات تجريبية
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Cars";
            cells["A4"].Value = "Bikes";
            cells["A5"].Value = "Cars";
            
            cells["B1"].Value = "Region";
            cells["B2"].Value = "North";
            cells["B3"].Value = "South";
            cells["B4"].Value = "North";
            cells["B5"].Value = "South";
            
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة الحقول وتكوين DragToPage
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField regionField = pivotTable.PageFields[fieldIndex];
            
            // عرض خاصية DragToPage
            regionField.DragToPage = false; // Disable dragging to page area
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحديث جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ دفتر العمل
            workbook.Save("PivotFieldDragToPageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


