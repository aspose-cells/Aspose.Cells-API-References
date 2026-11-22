---
title: "GlobalizationSettings.GetPivotTotalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم تسمية \\\"Total\\\" في الجدول المحوري. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي الجدول المحوري على حقلين محوريين أو أكثر في منطقة البيانات"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getpivottotalname/
---
## GlobalizationSettings.GetPivotTotalName method

تحصل على اسم تسمية \"Total\" في الجدول المحوري. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي الجدول المحوري على حقلين محوريين أو أكثر في منطقة البيانات.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotTotalName()
```

### قيمة الإرجاع

اسم تسمية \"Total\"

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotTotalNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "North"; worksheet.Cells["B2"].Value = 1000; worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "South"; worksheet.Cells["B3"].Value = 2000; worksheet.Cells["C3"].Value = 70;
            worksheet.Cells["A4"].Value = "West"; worksheet.Cells["B4"].Value = 3000; worksheet.Cells["C4"].Value = 110;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E5", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Quantity

            // إنشاء وتكوين إعدادات التعميم
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // إظهار استدعاء الطريقة مباشرة
                Console.WriteLine("Custom Total Name: " + customSettings.GetPivotTotalName());

                // معالجة الجدول المحوري
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Pivot table created with custom total name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetPivotTotalNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetPivotTotalName()
        {
            return "Custom Total";
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


