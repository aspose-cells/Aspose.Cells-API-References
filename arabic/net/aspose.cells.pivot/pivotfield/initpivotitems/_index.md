---
title: "PivotField.InitPivotItems"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تهيئة عناصر المحور للحقل المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/initpivotitems/
---
## PivotField.InitPivotItems method

تهيئة عناصر المحور للحقل المحوري

```csharp
[Obsolete("Please simply remove calling this method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void InitPivotItems()
```

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن غير صالحة. يرجى ببساطة إزالة استدعاء هذه الطريقة. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ أكتوبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodInitPivotItemsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // تهيئة عناصر المحور
                pivotField.InitPivotItems();

                // عرض عناصر المحور
                Console.WriteLine("Pivot Items after initialization:");
                foreach (PivotItem item in pivotField.PivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // احفظ المصنف
                workbook.Save("PivotFieldInitPivotItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitPivotItems method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


