---
title: "PivotField.IsHiddenItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تشير إلى ما إذا كان PivotItem المحدد مخفيًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/ishiddenitem/
---
## PivotField.IsHiddenItem method

تشير إلى ما إذا كان PivotItem المحدد مخفيًا.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItem(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس pivotItem في pivotField. |

### قيمة الإرجاع

ما إذا كان PivotItem المحدد مخفيًا

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.PivotItems[int].IsHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Country";
            worksheet.Cells["A2"].Value = "USA";
            worksheet.Cells["A3"].Value = "Canada";
            worksheet.Cells["A4"].Value = "UK";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[0];
            
            // إخفاء العنصر في الفهرس 1 (كندا)
            rowField.HideItem(1, true);
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // تحقق مما إذا كان العنصر في الفهرس 1 مخفيًا
            bool isHidden = rowField.IsHiddenItem(1);
            Console.WriteLine("Is item at index 1 hidden? " + isHidden);
            
            // احفظ المصنف
            workbook.Save("PivotFieldIsHiddenItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


