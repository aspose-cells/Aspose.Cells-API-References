---
title: "WebExtensionBinding.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionBinding. تحصل وتضبط معرف الربط"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

يحصل ويضبط معرف الربط.

```csharp
public string Id { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyIdDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة جديدة من WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // ضبط خاصية Id
                binding.Id = "SampleBindingId";
                
                // عرض القيمة الحالية لـ Id
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // تعديل قيمة Id لإظهار أنها قابلة للقراءة/الكتابة
                binding.Id = "UpdatedBindingId";
                Console.WriteLine("Updated Id value: " + binding.Id);
                
                Console.WriteLine("Id property has been successfully demonstrated");
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

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


