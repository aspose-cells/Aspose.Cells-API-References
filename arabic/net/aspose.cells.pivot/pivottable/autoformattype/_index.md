---
title: "PivotTable.AutoFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل وتضبط نوع التنسيق التلقائي لـ PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

يحصل على نوع التنسيق التلقائي لـ PivotTable ويضبطه.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutoFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Chair");
            worksheet.Cells["C4"].PutValue(150);
            
            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة حقول إلى المناطق
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
            
            // عرض خاصية AutoFormatType
            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report6;
            
            // احفظ المصنف
            workbook.Save("PivotTableAutoFormatTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


