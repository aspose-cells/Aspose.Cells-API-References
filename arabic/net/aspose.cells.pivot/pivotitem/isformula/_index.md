---
title: "PivotItem.IsFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

يشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotItem.IsCalculatedItem. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من نوفمبر 2024. Aspose يعتذر عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احصل على العنصر المحوري الأول
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // اعرض القيمة الحالية لخاصية IsFormula (خاصية مهجورة)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // عيّن قيمة جديدة لخاصية IsFormula (خاصية مهجورة)
            pivotItem.IsFormula = true;

            // عرض التأثير - سيؤدي ذلك إلى وضع علامة على العنصر المحوري كعنصر صيغة
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // ملاحظة: في الاستخدام الفعلي، يجب عليك استخدام IsCalculatedItem بدلاً من ذلك لأن IsFormula قد عُدِم.
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // حفظ النتيجة
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


