---
title: "PivotFilter.ValueFieldIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilter. تحصل على فهرس حقل القيمة في منطقة القيمة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/valuefieldindex/
---
## PivotFilter.ValueFieldIndex property

يحصل على فهرس حقل القيمة في منطقة القيمة.

```csharp
public int ValueFieldIndex { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValueFieldIndexDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
            
            // إضافة مرشح عد إلى حقل الصف
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // احصل على المرشح ووضح ValueFieldIndex
            PivotFilter filter = rowField.GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            
            // احفظ المصنف
            workbook.Save("PivotFilterValueFieldIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


