---
title: "PivotField.ClearFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. يزيل إعداد الفلتر على هذا الحقل المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

يمسح إعداد الفلتر على هذا الحقل المحوري.

```csharp
public void ClearFilter()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // طبق فلترًا أولاً لتوضيح إزالته
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // استدعِ طريقة ClearFilter
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // قم بتحديث الجدول المحوري لإظهار التغييرات
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


