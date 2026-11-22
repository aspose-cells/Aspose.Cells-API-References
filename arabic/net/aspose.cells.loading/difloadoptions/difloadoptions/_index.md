---
title: "DifLoadOptions.DifLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DifLoadOptions. الخيارات"
type: docs
url: /ar/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

الخيارات.

```csharp
public DifLoadOptions()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة جديدة من DifLoadOptions باستخدام المنشئ بدون معلمات
                DifLoadOptions loadOptions = new DifLoadOptions();

                // إنشاء مصنف جديد بخيارات افتراضية
                Workbook workbook = new Workbook();

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];

                // إضافة بيانات عينة لإظهار أن المصنف يعمل بشكل صحيح
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // احفظ المصنف بتنسيق DIF
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // الآن قم بتحميل ملف DIF المحفوظ باستخدام DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // احفظ البيانات المحمّلة إلى XLSX للتحقق
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


