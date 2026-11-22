---
title: "الفئة PivotTableCalculateOption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotTableCalculateOption. تمثل خيارات حساب بيانات جدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

يمثل خيارات حساب بيانات جدول محوري.

```csharp
public class PivotTableCalculateOption
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | يشير إلى ما إذا كان تحديث المخططات يعتمد على جدول المحور هذا. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | يشير إلى ما إذا كان تحديث مصدر البيانات لجدول المحور. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | يحصل على ويضبط خيارات تحديث مصدر البيانات إلى ذاكرة التخزين المؤقت للجدول المحوري. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | تمثل طريقة حجز العناصر المفقودة في pivot. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات لجدول المحور
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // تكوين جدول المحور
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // إنشاء كائن PivotTableCalculateOption
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // حساب بيانات جدول المحور باستخدام الخيارات المحددة
            pivotTable.CalculateData(calculateOption);

            // احفظ المصنف
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


