---
title: "IFilePathProvider.GetFullName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IFilePathProvider. تحصل على المسار الكامل للملف بواسطة اسم Worksheet عند تصدير Worksheet إلى HTML بشكل منفصل. وبالتالي يمكن تصدير المراجع بين Worksheets بشكل صحيح"
type: docs
url: /ar/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

يحصل على المسار الكامل للملف حسب اسم ورقة العمل عند تصدير ورقة العمل إلى HTML بشكل منفصل. وبالتالي يمكن تصدير المراجع بين أوراق العمل بشكل صحيح.

```csharp
public string GetFullName(string sheetName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | String | اسم Worksheet |

### قيمة الإرجاع

المسار الكامل للملف

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء تنفيذ مخصص لـ IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // استدعِ طريقة GetFullName مع اسم ورقة
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // اعرض النتيجة
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // تنفيذ بسيط يُرجع مسارًا يجمع بين اسم الورقة ودليل
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### انظر أيضًا

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


