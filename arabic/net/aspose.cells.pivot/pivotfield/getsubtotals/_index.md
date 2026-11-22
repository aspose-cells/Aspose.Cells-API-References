---
title: "PivotField.GetSubtotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تشير إلى ما إذا كان يجب عرض المجموع الفرعي المحدد لهذا حقل المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

يشير إلى ما إذا كان يجب إظهار المجموع الفرعي المحدد لهذا الحقل المحوري.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | نوع المجموع الفرعي. |

### قيمة الإرجاع

يرجع ما إذا كان يتم عرض المجموع الفرعي المحدد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // تحقق مما إذا كان المجموع الفرعي Sum مفعلاً
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // تحقق مما إذا كان المجموع الفرعي Average مفعلاً
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // تمكين المجموع الفرعي Sum
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // تحقق من أن المجموع الفرعي Sum مفعّل الآن
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // قم بتحديث الجدول المحوري لإظهار التغييرات
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


