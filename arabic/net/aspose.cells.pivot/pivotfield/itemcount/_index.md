---
title: "PivotField.ItemCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تحصل على عدد العناصر الأساسية في هذا الحقل المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

يحصل على عدد العناصر الأساسية في هذا الحقل المحوري.

```csharp
[Obsolete("Use PivotField.PivotItems.Count instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ItemCount { get; }
```

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.PivotItems.Count بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["A6"].PutValue("Fruit");
            worksheet.Cells["A7"].PutValue("Vegetable");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(120);
            worksheet.Cells["B6"].PutValue(180);
            worksheet.Cells["B7"].PutValue(90);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // حساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احصل على الحقل المحوري وعرض عدد عناصره
            PivotField pivotField = pivotTable.RowFields[0];
            Console.WriteLine("Item count in pivot field: " + pivotField.ItemCount);
            
            // احفظ المصنف
            workbook.Save("PivotFieldItemCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


