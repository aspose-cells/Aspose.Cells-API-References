---
title: "PivotItem.PositionInSameParentNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تحديد فهرس الموضع في PivotItems تحت نفس العقدة الأصلية"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/positioninsameparentnode/
---
## PivotItem.PositionInSameParentNode property

تحديد فهرس الموضع في PivotItems تحت نفس العقدة الأصلية.

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int PositionInSameParentNode { get; set; }
```

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.MoveItem(PivotFieldType, string[],bool,int). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2026. Aspose يعتذر عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionInSameParentNodeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // أضف ورقة عمل جديدة للجدول المحوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // إضافة جدول محوري
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // تكوين جدول محوري
            PivotField vendorField = pivotTable.RowFields["Vendor"];
            vendorField.SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // تحديث وحساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // عرض خاصية PositionInSameParentNode
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // تعيين المواضع داخل نفس العقدة الأصلية
            items["4H12"].PositionInSameParentNode = 1;
            items["DIF400"].PositionInSameParentNode = 2;
            
            // إعادة الحساب بعد تغيير المواضع
            pivotTable.CalculateData();
            
            // تعيين المواضع لمجموعة أخرى
            items["CA32"].PositionInSameParentNode = 1;
            items["AAA3"].PositionInSameParentNode = 2;

            // احفظ المصنف
            workbook.Save("PivotTableWithPositionInSameParentNode.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


