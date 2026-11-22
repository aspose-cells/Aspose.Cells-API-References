---
title: "Enum PivotItemPositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotItemPositionType enum. يمثل نوع الموضع لعنصر الأساس المحوري في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

يمثل نوع الموضع لعنصر الأساس pivot في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام.

```csharp
public enum PivotItemPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Previous | `0` | يمثل العنصر المحوري السابق في PivotField. |
| Next | `1` | يمثل العنصر المحوري التالي في PivotField. |
| Custom | `2` | يعرض القيم بصيغة مختلفة بناءً على فهرس العنصر المحوري في PivotField. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
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

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // حدد صيغة عرض البيانات لإظهار القيم كفرق عن العنصر السابق
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // تحديث وحساب جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


