---
title: "LoadFilter.LoadDataFilterOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadFilter. خيارات الفلتر لتحديد ما البيانات التي يجب تحميلها"
type: docs
url: /ar/net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

خيارات الفلتر لتحديد البيانات التي يجب تحميلها.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = 123;
            worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

            try
            {
                // إنشاء مثال LoadFilter مع الخيارات الافتراضية
                LoadFilter loadFilter = new LoadFilter();

                // عرض قيمة LoadDataFilterOptions الافتراضية
                Console.WriteLine("Default LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // تعيين خيارات فلتر جديدة (تجميع للعلامات)
                loadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellValue | LoadDataFilterOptions.Formula;

                // عرض القيمة المحدثة
                Console.WriteLine("Updated LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // إنشاء فلتر آخر بخيارات مختلفة
                LoadFilter anotherFilter = new LoadFilter(LoadDataFilterOptions.Chart | LoadDataFilterOptions.Picture);

                // عرض الخيارات من المُنشئ
                Console.WriteLine("Constructor LoadDataFilterOptions: " + anotherFilter.LoadDataFilterOptions);

                // احفظ المصنف
                workbook.Save("LoadDataFilterOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


