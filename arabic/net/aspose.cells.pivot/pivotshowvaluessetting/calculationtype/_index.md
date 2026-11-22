---
title: "PivotShowValuesSetting.CalculationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotShowValuesSetting. تمثل طريقة إظهار قيم حقل البيانات في تقرير المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

تمثل طريقة إظهار قيم حقل البيانات في تقرير المحور.

```csharp
[Obsolete("Use PivotShowValuesSetting.ShowValuesAs property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotShowValuesSetting.ShowValuesAs. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyCalculationTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
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

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // أضف حقل البيانات وحدد نوع الحساب
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.RankLargestToSmallest;

            // احسب البيانات واحفظها
            pivotTable.CalculateData();
            workbook.Save("PivotShowValuesSettingPropertyCalculationTypeDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


