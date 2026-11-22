---
title: "PivotTable.MissingItemsLimit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مُعينة عليها"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/missingitemslimit/
---
## PivotTable.MissingItemsLimit property

يحدد قيمة منطقية تشير إلى ما إذا كانت حقول PivotTable يمكن أن تحتوي على فلاتر متعددة مضبوطة عليها.

```csharp
[Obsolete("Use PivotCache.MissingItemsLimit propery  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotMissingItemLimitType MissingItemsLimit { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotCache.MissingItemsLimit. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMissingItemsLimitDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // بيانات عينة
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 30;

            // أنشئ جدولًا محوريًا واحصل على المثيل
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "E3");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
            
            // عرض خاصية MissingItemsLimit
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.Max;
            
            // تحديث البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotTableMissingItemsLimitDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotMissingItemLimitType](../../pivotmissingitemlimittype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


