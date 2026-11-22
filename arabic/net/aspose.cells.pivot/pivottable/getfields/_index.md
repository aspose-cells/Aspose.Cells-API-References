---
title: "PivotTable.GetFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تحصل على قائمة الحقول Pivot المحددة حسب المنطقة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/getfields/
---
## PivotTable.GetFields method

يحصل على قائمة حقول المحور المحددة حسب المنطقة.

```csharp
public PivotFieldCollection GetFields(PivotFieldType fieldType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع المنطقة. |

### قيمة الإرجاع

مجموعة الحقول Pivot المحددة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodGetFieldsWithPivotFieldTypeDemo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // استدعاء طريقة GetFields مع معامل PivotFieldType.Row
                PivotFieldCollection rowFields = pivotTable.GetFields(PivotFieldType.Row);
                
                Console.WriteLine($"Number of row fields: {rowFields.Count}");
                foreach (PivotField field in rowFields)
                {
                    Console.WriteLine($"Row field name: {field.Name}");
                }

                // استدعاء طريقة GetFields مع معامل PivotFieldType.Data
                PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
                
                Console.WriteLine($"Number of data fields: {dataFields.Count}");
                foreach (PivotField field in dataFields)
                {
                    Console.WriteLine($"Data field name: {field.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFields method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotTableGetFieldsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


