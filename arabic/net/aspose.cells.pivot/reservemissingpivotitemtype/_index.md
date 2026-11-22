---
title: "تعداد ReserveMissingPivotItemType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.ReserveMissingPivotItemType enum. يمثل كيفية الاحتفاظ بعناصر المحور المفقودة"
type: docs
url: /ar/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

يمثل طريقة الاحتفاظ بالعناصر المفقودة في pivot.

```csharp
public enum ReserveMissingPivotItemType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | يزيل عناصر المحور المفقودة القديمة ويحتفظ بالعناصر المحذوفة من مصدر البيانات الجديد كعناصر مفقودة. |
| All | `1` | يحتفظ بجميع العناصر المفقودة. |
| None | `2` | يزيل جميع عناصر المحور المفقودة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة PivotTable إلى ورقة العمل
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // إضافة حقول إلى PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // تعيين خيار ReserveMissingPivotItemType
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // حساب PivotTable باستخدام الخيارات المحددة
            pivotTable.CalculateData(calculateOption);

            // تحديث PivotTable
            pivotTable.RefreshData();

            // احفظ المصنف
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


