---
title: "WorkbookSettings.MaxUniqueItemsPerField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل وتعيّن حد العناصر الفريدة لكل حقل"
type: docs
url: /ar/net/aspose.cells/workbooksettings/maxuniqueitemsperfield/
---
## WorkbookSettings.MaxUniqueItemsPerField property

يحصل أو يضبط حد العناصر الفريدة لكل حقل

```csharp
public int MaxUniqueItemsPerField { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertyMaxUniqueItemsPerFieldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            try
            {
                // عرض قيمة MaxUniqueItemsPerField الحالية
                Console.WriteLine("Current MaxUniqueItemsPerField value: " + settings.MaxUniqueItemsPerField);

                // عرض تعيين قيمة جديدة لـ MaxUniqueItemsPerField
                settings.MaxUniqueItemsPerField = 1000;
                Console.WriteLine("After setting to 1000: " + settings.MaxUniqueItemsPerField);

                // تعيين قيمة أخرى لإظهار أنه قابل للتغيير
                settings.MaxUniqueItemsPerField = 5000;
                Console.WriteLine("After setting to 5000: " + settings.MaxUniqueItemsPerField);

                // أضف بعض البيانات النموذجية لجعل المثال ذو معنى
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Orange");

                // احفظ المصنف
                workbook.Save("MaxUniqueItemsPerFieldDemo.xlsx");
                Console.WriteLine("Workbook saved with MaxUniqueItemsPerField settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


