---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم رأس حقل منطقة القيمة في PivotTable"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

يحصل على اسم رأس حقل منطقة القيمة في PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### قيمة الإرجاع

اسم رأس حقل البيانات

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية لـ PivotTable
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // تعيين إعدادات العولمة المخصصة
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // إنشاء PivotTable وتكوين الحقول
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // تحديث PivotTable لتطبيق تغييرات التعريب
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // تنفيذ مخصص لـ GlobalizationSettings
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


