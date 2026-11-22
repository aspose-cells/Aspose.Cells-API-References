---
title: "PivotShowValuesSetting.BaseItemIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotShowValuesSetting. تمثل الفهرس المخصص للعنصر المحوري في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام"
type: docs
url: /ar/net/aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/
---
## PivotShowValuesSetting.BaseItemIndex property

تمثل الفهرس المخصص لعنصر الـ Pivot في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام.

```csharp
public int BaseItemIndex { get; set; }
```

### ملاحظات

[`PreviousPivotItem`](../previouspivotitem/) (-1) for the preceding item, [`NextPivotItem`](../nextpivotitem/) (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyBaseItemIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تكوين إعدادات إظهار القيم
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;
            dataField.ShowValuesSetting.BaseFieldIndex = 0;
            dataField.ShowValuesSetting.BaseItemIndex = 1; // Using BaseItemIndex property

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            workbook.Save("PivotShowValuesSettingBaseItemIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


