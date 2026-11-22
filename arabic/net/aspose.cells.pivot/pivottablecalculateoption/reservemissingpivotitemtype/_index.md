---
title: "PivotTableCalculateOption.ReserveMissingPivotItemType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTableCalculateOption. تمثل طريقة حجز العناصر المحورية المفقودة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/
---
## PivotTableCalculateOption.ReserveMissingPivotItemType property

تمثل طريقة حجز العناصر المفقودة في pivot.

```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```

### ملاحظات

تعمل فقط عندما يكون [`RefreshData`](../refreshdata/) صحيحًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // بيانات عينة
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(30);

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // تكوين حقول المحور
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // ضبط خيارات الحساب باستخدام ReserveMissingPivotItemType
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // احسب باستخدام الخيارات
            pivotTable.CalculateData(options);

            // حفظ النتيجة
            workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


