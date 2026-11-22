---
title: "PivotField.HideItemDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تحدد ما إذا كان PivotItem المحدد في حقل محوري مخفيًا بالتفصيل"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

تحدد ما إذا كان PivotItem المحدد في حقل محوري مخفيًا بالتفصيل.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس pivotItem في pivotField. |
| isHiddenDetail | منطقي | ما إذا كان PivotItem المحدد مخفيًا |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.PivotItems[int].IsDetailHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقول إلى المناطق
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // إخفاء تفاصيل العنصر عند الفهرس 2 (East) مع isHidden=false
            pivotField.HideItemDetail(2, false);
            
            // تحديث وحساب بيانات جدول البيفوت
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


