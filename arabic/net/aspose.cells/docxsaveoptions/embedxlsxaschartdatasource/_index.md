---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocxSaveOptions. تشير إلى ما إذا كان سيتم تضمين ملف xlsx كمصدر بيانات للمخطط"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

يشير إلى ما إذا كان يتم تضمين ملف xlsx كمصدر بيانات للمخطط.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // تهيئة DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // اعرض القيمة الافتراضية لخاصية EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // عيّن EmbedXlsxAsChartDataSource إلى true لتوضيح استخدامه
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // حفظ المصنف كملف DOCX باستخدام الخيارات المكوّنة
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


