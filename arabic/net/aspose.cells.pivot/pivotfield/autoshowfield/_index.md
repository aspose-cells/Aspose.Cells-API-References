---
title: "PivotField.AutoShowField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تمثل فهرس الحقل العرض التلقائي. 1 يعني PivotField نفسه. يجب أن يكون فهرس حقول البيانات."
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/autoshowfield/
---
## PivotField.AutoShowField property

تمثل فهرس الحقل العرض التلقائي. -1 يعني PivotField نفسه. يجب أن يكون فهرس حقول البيانات.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.RankBy property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowField { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.RankBy أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // إضافة بيانات عينة لجدول محوري
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;
            
            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // تكوين AutoShow للحقل المحوري الأول
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.AutoShowCount = 2;
            pivotField.AutoShowField = 1; // Index of data field (Quantity)
            pivotField.IsAutoShow = true;
            pivotField.IsAscendShow = true; // Equivalent to "Top" in AutoShowType
            
            // احفظ المصنف
            workbook.Save("PivotField_AutoShowField_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


