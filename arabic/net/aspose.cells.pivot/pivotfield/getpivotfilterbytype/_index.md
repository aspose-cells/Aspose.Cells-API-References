---
title: "PivotField.GetPivotFilterByType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تحصل على مرشح الحقل المحوري حسب النوع."
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/getpivotfilterbytype/
---
## PivotField.GetPivotFilterByType method

يحصل على عامل تصفية المحور للحقل المحوري حسب النوع

```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetPivotFilterByTypeWithPivotFilterTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            
            sheet.Cells["B1"].Value = "Count";
            sheet.Cells["B2"].Value = 1;
            sheet.Cells["B3"].Value = 2;
            sheet.Cells["B4"].Value = 3;
            sheet.Cells["B5"].Value = 4;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // تطبيق مرشح العد.
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // احصل على مرشح العد.
            PivotFilter filter = rowField.GetPivotFilterByType(PivotFilterType.Count);
            
            // إخراج تفاصيل المرشح.
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            Console.WriteLine("Auto Filter: " + filter.AutoFilter);
            
            wb.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


