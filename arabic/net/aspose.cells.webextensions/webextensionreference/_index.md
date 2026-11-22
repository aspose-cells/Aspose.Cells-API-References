---
title: "الفئة WebExtensionReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WebExtensions.WebExtensionReference. تمثل تحديد موقع الموفر وإصدار الامتداد"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

يمثل تحديد موقع المزود وإصدار الامتداد.

```csharp
public class WebExtensionReference
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | يحصل ويضبط المعرف المرتبط بإضافة Office داخل موفر الفهرس. يجب أن يكون المعرف فريدًا داخل موفر الفهرس. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | يحصل ويضبط نسخة السوق التي تُخزن فيها إضافة Office. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | يحصل ويضبط نوع السوق الذي يحدده سمة المتجر. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | يحصل ويضبط الإصدار. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أنشئ WebExtension أولاً
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // احصل على WebExtensionReference من WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // اضبط خصائص WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // اعرض خصائص المرجع
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // احفظ المصنف
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


