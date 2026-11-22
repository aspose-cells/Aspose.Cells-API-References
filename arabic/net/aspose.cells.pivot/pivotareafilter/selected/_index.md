---
title: "PivotAreaFilter.Selected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotAreaFilter. تشير إلى ما إذا كان لهذا الحقل اختيار. تعمل فقط عندما يكون جدول المحور في وضع المخطط التفصيلي"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

يشير إلى ما إذا كان لهذا الحقل اختيار. يعمل فقط عندما يكون PivotTable في عرض المخطط التفصيلي.

```csharp
public bool Selected { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // احصل على فلتر منطقة المحور
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // عرض القيمة المحددة الحالية
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // تغيير القيمة المحددة (يؤثر فقط على وضع المخطط التفصيلي)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // احفظ المصنف
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


