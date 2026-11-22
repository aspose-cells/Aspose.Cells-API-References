---
title: "SaveOptions.SortExternalNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تشير إلى ما إذا كان يتم فرز الأسماء المعرفة خارجيًا قبل حفظ الملف"
type: docs
url: /ar/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

```csharp
public bool SortExternalNames { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء كائن OoxmlSaveOptions يرث من SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // عرض القيمة الافتراضية لخاصية SortExternalNames
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // تعيين SortExternalNames إلى true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // احفظ المصنف باستخدام خيارات الحفظ المحددة
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


