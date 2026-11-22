---
title: "PivotItem.IsHideDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تحصل وتضبط ما إذا كان عنصر Pivot يخفي التفاصيل"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/ishidedetail/
---
## PivotItem.IsHideDetail property

تحصل وتضبط ما إذا كان عنصر Pivot يخفي التفاصيل.

```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotItem.IsDetailHidden. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2024. تقدم Aspose اعتذارها عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHideDetailDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            foreach (PivotItem pivotItem in pivotItems)
            {
                Console.WriteLine($"Original IsHideDetail: {pivotItem.IsHideDetail}");
                pivotItem.IsHideDetail = true;
                Console.WriteLine($"Modified IsHideDetail: {pivotItem.IsHideDetail}");
            }

            workbook.Save("PivotItemIsHideDetailDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


