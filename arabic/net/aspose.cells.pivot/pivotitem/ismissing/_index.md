---
title: "PivotItem.IsMissing"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تشير إلى ما إذا كان العنصر قد أُزيل من مصدر البيانات"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

يشير إلى ما إذا تم إزالة العنصر من مصدر البيانات.

```csharp
public bool IsMissing { get; }
```

### ملاحظات

True يعني أن هذه القيمة قد أُزيلت من مصدر البيانات.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احصل على أول عنصر محور في حقل الصف الأول
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // عرض قيمة خاصية IsMissing
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // إنشاء سيناريو قد يكون فيه عنصر مفقودًا
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // تحقق مما إذا كان عنصر المحور الأصلي مفقودًا الآن
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // احفظ المصنف
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


