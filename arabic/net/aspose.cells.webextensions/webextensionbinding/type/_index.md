---
title: "WebExtensionBinding.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionBinding. تحصل وتضبط نوع الربط"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

يحصل ويضبط نوع الربط.

```csharp
public string Type { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة جديدة من WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // ضبط خاصية Type
                binding.Type = "text";
                
                // عرض القيمة الحالية لـ Type
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // تعديل قيمة Type لإظهار أنها قابلة للقراءة/الكتابة
                binding.Type = "range";
                Console.WriteLine("Updated Type value: " + binding.Type);
                
                Console.WriteLine("Type property has been successfully demonstrated");
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


