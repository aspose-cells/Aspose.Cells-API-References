---
title: "الفئة WebExtensionBinding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WebExtensions.WebExtensionBinding. تمثل علاقة ربط بين إضافة Office والبيانات في المستند"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

يمثل علاقة ربط بين Office Add-in والبيانات في المستند.

```csharp
public class WebExtensionBinding
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | يحصل ويضبط مفتاح الربط المستخدم لتعيين إدخال الربط في هذه القائمة مع البيانات المرتبطة في المستند. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | يحصل ويضبط معرف الربط. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | يحصل ويضبط نوع الربط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة جديدة من WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();

                // تعيين الخصائص
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // عرض قيم الخصائص
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // تعديل الخصائص
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


