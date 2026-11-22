---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. تحصل أو تعيين IFilePathProvider لتصدير Worksheet إلى html بشكل منفصل"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

يحصل على أو يضبط IFilePathProvider لتصدير Worksheet إلى html بشكل منفصل.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وإضافة بعض البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // إنشاء HtmlSaveOptions وتعيين FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // حفظ المصنف بتنسيق HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // منطق مخصص لإنشاء مسارات الملفات
            return $"custom_{sheetName}";
        }
    }
}
```

### انظر أيضًا

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


