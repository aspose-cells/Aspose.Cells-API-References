---
title: "Enum PivotFieldSubtotalType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType enum. وصف موجز لـ PivotFieldSubtotalType"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

وصف ملخص لـ PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يمثل نوع المجموع الفرعي None. |
| Automatic | `1` | يمثل نوع المجموع الفرعي Automatic. |
| Sum | `2` | يمثل نوع المجموع الفرعي Sum. |
| Count | `4` | يمثل نوع المجموع الفرعي Count. |
| Average | `8` | يمثل نوع المجموع الفرعي Average. |
| Max | `10` | يمثل نوع المجموع الفرعي Max. |
| Min | `20` | يمثل نوع المجموع الفرعي Min. |
| Product | `40` | يمثل نوع المجموع الفرعي Product. |
| CountNums | `80` | يمثل نوع المجموع الفرعي لـ Count Nums. |
| Stdev | `100` | يمثل نوع المجموع الفرعي للانحراف المعياري. |
| Stdevp | `200` | يمثل نوع المجموع الفرعي للانحراف المعياري للسكان. |
| Var | `400` | يمثل نوع المجموع الفرعي للتباين. |
| Varp | `800` | يمثل نوع المجموع الفرعي لتباين السكان. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // إضافة جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // تعيين نوع المجموع الفرعي لحقل الصف
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // تحديث وحساب بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


