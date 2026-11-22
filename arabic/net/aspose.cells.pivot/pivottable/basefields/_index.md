---
title: "PivotTable.BaseFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُرجع جميع حقول المحور الأساسية في PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

يرجع جميع حقول Pivot الأساسية في PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyBaseFieldsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // الوصول إلى مجموعة BaseFields
            PivotFieldCollection baseFields = pivotTable.BaseFields;
            
            // عرض العناصر الأصلية من كل حقل أساسي
            Console.WriteLine("Base Fields and their Original Items:");
            foreach (PivotField field in baseFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                string[] originalItems = field.OriginalItems;
                foreach (string item in originalItems)
                {
                    Console.WriteLine($"- {item}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


