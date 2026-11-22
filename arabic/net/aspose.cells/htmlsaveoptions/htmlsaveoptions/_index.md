---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ HtmlSaveOptions. ينشئ خيارات لحفظ ملف html"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

ينشئ خيارات لحفظ ملف html.

```csharp
public HtmlSaveOptions()
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // تهيئة HtmlSaveOptions باستخدام المنشئ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // حفظ كـ HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved to: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

ينشئ خيارات لحفظ ملف htm.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | SaveFormat | تنسيق الملف. يجب أن يكون أحد الأنواع التالية: Html أو MHtml، وإلا سيتم تعيين تنسيق الحفظ تلقائيًا إلى Html |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            try
            {
                // إنشاء HtmlSaveOptions مع معامل SaveFormat
                HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
                
                // تعيين بعض الخصائص
                saveOptions.PageTitle = "Aspose.Cells HTML Export";
                saveOptions.ExportActiveWorksheetOnly = true;
                saveOptions.ExportGridLines = true;
                
                // حفظ المصنف باستخدام HtmlSaveOptions
                workbook.Save("HtmlExportWithOptions.html", saveOptions);
                
                Console.WriteLine("HTML file saved successfully with HtmlSaveOptions(SaveFormat)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HtmlSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


