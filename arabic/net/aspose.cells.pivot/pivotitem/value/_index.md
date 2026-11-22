---
title: "PivotItem.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تحصل على قيمة عنصر Pivot"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/value/
---
## PivotItem.Value property

يحصل على قيمة العنصر المحوري

```csharp
public object Value { get; }
```

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyValueDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // معالجة عناصر Pivot
            List<string> valuesToShow = new List<string> { "Apple", "Banana" };
            
            Console.WriteLine("Pivot Items Before Filtering:");
            PrintPivotItems(pivotField);

            // تصفية عناصر Pivot بناءً على خاصية Value
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                string itemValue = item.Value?.ToString() ?? "";
                
                if (!valuesToShow.Contains(itemValue))
                {
                    item.IsHidden = true;
                }
            }

            Console.WriteLine("\nPivot Items After Filtering:");
            PrintPivotItems(pivotField);
        }

        private static void PrintPivotItems(PivotField pivotField)
        {
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                Console.WriteLine($"Name: {item.Name}, Value: {item.Value}, Hidden: {item.IsHidden}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


