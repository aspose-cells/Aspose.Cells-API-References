---
title: "PivotItem.IsCalculatedItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

يشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة.

```csharp
public bool IsCalculatedItem { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // حساب بيانات جدول المحور
            pivotTable.CalculateData();

            // احصل على العنصر المحوري الأول من الحقل المحوري الأول
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // اعرض قيمة خاصية IsCalculatedItem
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // تحقق مما إذا كان العنصر المحوري عنصرًا محسوبًا
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // احفظ المصنف
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


