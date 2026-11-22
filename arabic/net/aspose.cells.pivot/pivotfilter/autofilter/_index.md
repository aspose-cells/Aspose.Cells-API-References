---
title: "PivotFilter.AutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilter. تحصل على الفلتر التلقائي لمرشح المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/autofilter/
---
## PivotFilter.AutoFilter property

يحصل على الفلتر التلقائي لمرشح المحور.

```csharp
[Obsolete("Use FilterLabel, FilterValue,FilterDate or FilterTop10 method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter AutoFilter { get; }
```

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الطريقة FilterLabel أو FilterValue أو FilterDate أو FilterTop10. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تُعرب Aspose عن اعتذارها عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // إضافة مرشح إلى جدول pivot
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.PageFields[0];

            // إنشاء وإضافة مرشح
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];

            try
            {
                // عرض قيمة خاصية AutoFilter (للقراءة فقط)
                Console.WriteLine("AutoFilter Range: " + filter.AutoFilter.Range);
                Console.WriteLine("AutoFilter ShowFilterButton: " + filter.AutoFilter.ShowFilterButton);

                // عرض كيفية الوصول إلى خصائص AutoFilter
                Console.WriteLine("AutoFilter has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("PivotFilterAutoFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


