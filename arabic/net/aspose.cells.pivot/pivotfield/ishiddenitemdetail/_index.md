---
title: "PivotField.IsHiddenItemDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تشير إلى ما إذا كان يجب إخفاء تفاصيل PivotItem المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

تشير إلى ما إذا كان يجب إخفاء تفاصيل PivotItem المحدد..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس pivotItem في pivotField. |

### قيمة الإرجاع

ما إذا كان تفاصيل PivotItem المحدد مخفية

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.PivotItems[int].IsDetailHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // احصل على حقل المحور
            PivotField pivotField = pivotTable.RowFields[0];
            
            // إخفاء تفاصيل العنصر للمؤشر 1 (USA)
            pivotField.HideItemDetail(1, true);
            
            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // تحقق مما إذا كانت تفاصيل العنصر مخفية
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // احفظ دفتر العمل
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


