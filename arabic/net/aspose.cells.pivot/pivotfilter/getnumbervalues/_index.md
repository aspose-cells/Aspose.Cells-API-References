---
title: "PivotFilter.GetNumberValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFilter. تحصل على قيم مرشح الأعداد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/getnumbervalues/
---
## PivotFilter.GetNumberValues method

يحصل على قيم مرشح الأعداد.

```csharp
public double[] GetNumberValues()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetNumberValuesDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 5;
            sheet.Cells["B3"].Value = 3;
            sheet.Cells["B4"].Value = 2;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // تطبيق مرشح القيمة
            pivotTable.RowFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 4, 0);
            
            // احصل على قيم المرشح وعرضها
            PivotFilter filter = pivotTable.RowFields[0].GetFilters()[0];
            double[] numberValues = filter.GetNumberValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Number Values: " + string.Join(", ", numberValues));
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


