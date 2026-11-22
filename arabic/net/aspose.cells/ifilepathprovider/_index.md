---
title: "الواجهة IFilePathProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.IFilePathProvider. تمثل موفر مسار الملف المُصدَّر"
type: docs
url: /ar/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

يمثل موفر مسار الملف المُصدّر.

```csharp
public interface IFilePathProvider
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | يحصل على المسار الكامل للملف حسب اسم ورقة العمل عند تصدير ورقة العمل إلى HTML بشكل منفصل. وبالتالي يمكن تصدير المراجع بين أوراق العمل بشكل صحيح. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // تنفيذ طريقة GetFullName من واجهة IFilePathProvider
        public string GetFullName(string sheetName)
        {
            // للتوضيح، إرجاع مسار ملف بسيط بناءً على اسم الورقة
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // إنشاء مصنف جديد وإضافة بعض البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // إنشاء HtmlSaveOptions وتعيين FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // حفظ المصنف بتنسيق HTML
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


