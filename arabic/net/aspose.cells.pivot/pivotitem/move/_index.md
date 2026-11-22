---
title: "PivotItem.Move"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotItem. ينقل العنصر للأعلى أو للأسفل"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

ينقل العنصر للأعلى أو للأسفل

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| إزاحة | Int32 | عدد التحركات للأعلى أو للأسفل. حرك العنصر للأعلى إذا كان هذا أقل من الصفر؛ حرك العنصر للأسفل إذا كان هذا أكبر من الصفر. |
| isSameParent | منطقي | تحديد ما إذا كانت عملية النقل في نفس العقدة الأصلية أم لا |

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام PivotTable.MoveItem(PivotFieldType, string[],bool,int) أو طريقة PivotItem.Move(int) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // احصل على العناصر المحورية وعرض طريقة Move
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // نقل العنصر الأول إلى الموضع 1 (الموضع الثاني) مع العناصر الفرعية
            items[0].Move(1, true);
            
            // احفظ المصنف
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

ينقل العنصر للأعلى أو للأسفل في حقل المحور

```csharp
public void Move(int offset)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| إزاحة | Int32 | عدد التحركات للأعلى أو للأسفل. حرك العنصر للأعلى إذا كان هذا أقل من الصفر؛ حرك العنصر للأسفل إذا كان هذا أكبر من الصفر. |

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


