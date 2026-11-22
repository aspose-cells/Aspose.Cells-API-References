---
title: "PivotTable.FormatRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "PivotTable method. تنسيق بيانات الصف في منطقة PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/formatrow/
---
## PivotTable.FormatRow method

تنسيق بيانات الصف في منطقة جدول المحور

```csharp
public void FormatRow(int row, Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف لكائن Row |
| النمط | النمط | النمط الذي سيتم تنسيقه |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatRowWithInt32StyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // بيانات عينة لجدول pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // إنشاء نمط للتنسيق
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            
            // العثور على الصفوف وتنسيقها
            Cell cell = worksheet.Cells.Find("A", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            cell = worksheet.Cells.Find("B", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            // احفظ المصنف
            wb.Save("PivotTableFormatRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


