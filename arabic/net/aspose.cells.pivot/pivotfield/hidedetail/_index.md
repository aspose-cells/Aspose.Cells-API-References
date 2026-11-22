---
title: "PivotField.HideDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تحدد ما إذا كان تفاصيل جميع PivotItems في حقل محوري مخفيًا. أي طي/توسيع هذا الحقل"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

تحدد ما إذا كان تفاصيل جميع PivotItems في حقل محوري مخفيًا. أي طي/توسيع هذا الحقل.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isHiddenDetail | منطقي | ما إذا كان سيتم إخفاء تفاصيل حقل المحور. |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotItemsCollection.HideAllDetails() و UnhideAllDetails(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // إخفاء التفاصيل لحقل الصف الأول
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


