---
title: "PivotField.AutoShowCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/autoshowcount/
---
## PivotField.AutoShowCount property

يمثل عدد العناصر العليا أو السفلى التي يتم عرضها تلقائيًا في حقل PivotTable المحدد.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.AutoShowCount property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowCount { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.AutoShowCount أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowCountDemo
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
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 25;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقل صف وتعيين خصائص AutoShow
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.AutoShowCount = 2;
            rowField.IsAutoShow = true;
            rowField.AutoShowField = 1; // Index of "Quantity" field (0-based)

            // احسب البيانات واحفظها
            pivotTable.CalculateData();
            workbook.Save("PivotFieldAutoShowCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


