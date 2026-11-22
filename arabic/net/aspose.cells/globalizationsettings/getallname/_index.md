---
title: "GlobalizationSettings.GetAllName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. يحصل على اسم التسمية All في PivotTable"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getallname/
---
## GlobalizationSettings.GetAllName method

يحصل على اسم التسمية "(All)" في PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfAll() method instead.")]
public virtual string GetAllName()
```

### قيمة الإرجاع

اسم التسمية "(All)"

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة GlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetAllNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد بإعدادات عولمة مخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // الوصول إلى نسخة الإعدادات المخصصة
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            try
            {
                // استدعِ طريقة GetAllName وعرض النتيجة
                string allName = settings.GetAllName();
                Console.WriteLine($"Custom (All) label: {allName}");

                // إنشاء جدول محوري تجريبي لتوضيح تأثير التعريب
                Worksheet worksheet = workbook.Worksheets[0];
                CreateSampleData(worksheet);
                CreatePivotTable(worksheet);

                Console.WriteLine("Demo executed successfully. Check output file's pivot table labels.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("MethodGetAllNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // إنشاء بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Cars";
            worksheet.Cells["A4"].Value = "Bikes";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["B4"].Value = 1500;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // إنشاء جدول محوري باستخدام بيانات تجريبية
            int pivotIndex = worksheet.PivotTables.Add(
                "PivotTable",
                "A1:B4",
                "E3"
            );
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // تكوين بنية الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[0]); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[1]); // Sales

            // تحديث الجدول لتطبيق إعدادات التعريب
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetAllName()
        {
            // تنفيذ مخصص يُعيد العلامة "All" المترجمة
            return "[Custom All Selection]";
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


