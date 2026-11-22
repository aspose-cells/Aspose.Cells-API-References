---
title: "GlobalizationSettings.GetPivotGrandTotalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تُحصل على اسم تسمية Grand Total في الجدول المحوري"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getpivotgrandtotalname/
---
## GlobalizationSettings.GetPivotGrandTotalName method

يحصل على اسم تسمية "Grand Total" في الجدول المحوري.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfGrandTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotGrandTotalName()
```

### قيمة الإرجاع

اسم تسمية "Grand Total"

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotGrandTotalNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين إعدادات العولمة المخصصة
            var settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // ملء بيانات تجريبية للجدول المحوري
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Q1";
            cells["C1"].Value = "Q2";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1500;
            cells["C2"].Value = 2200;
            cells["A3"].Value = "Clothing";
            cells["B3"].Value = 900;
            cells["C3"].Value = 1300;

            // إنشاء جدول محوري مع حقول بيانات متعددة
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C3", "E4");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Q1
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Q2

            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            try
            {
                // عرض استدعاء GetPivotGrandTotalName
                string grandTotalName = settings.GetPivotGrandTotalName();
                Console.WriteLine($"Custom Grand Total Name: {grandTotalName}");

                // حفظ المصنف المعدل
                workbook.Save("GlobalizationSettingsMethodGetPivotGrandTotalNameDemo.xlsx");
                Console.WriteLine("Spreadsheet saved. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetPivotGrandTotalName()
            {
                return "[Custom Grand Total]";
            }
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


