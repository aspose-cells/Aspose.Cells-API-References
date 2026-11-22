---
title: "PivotField.AutoSortField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تمثّل فهرس الحقل الذي يتم فرزه تلقائيًا. 1 يعني PivotField نفسه، والقيم الأخرى تعني موقع حقول البيانات."
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

يمثّل فهرس الحقل الذي يتم فرزه تلقائيًا. -1 يعني PivotField نفسه، والقيم الأخرى تعني موقع حقول البيانات.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortBy أو طريقة PivotField.SortBy(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تُقدِّم Aspose اعتذارها عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // تكوين الفرز التلقائي.
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // حساب البيانات وتحديثها
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


