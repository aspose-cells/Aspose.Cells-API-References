---
title: "PivotTable.ChangeDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تغيير مصدر البيانات لجدول المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/changedatasource/
---
## PivotTable.ChangeDataSource method

غيّر مصدر البيانات لجدول المحور.

```csharp
public void ChangeDataSource(string[] source)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class PivotTableMethodChangeDataSourceWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحضير مصدر بيانات جديد
            string[] newDataSource = new string[] { "C1:D4", "Sheet1" };

            try
            {
                // تغيير مصدر البيانات لجدول المحوري
                pivotTable.ChangeDataSource(newDataSource);

                // تحديث جدول المحوري لتطبيق التغييرات
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable data source changed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing pivot table data source: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("PivotTableChangeDataSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


