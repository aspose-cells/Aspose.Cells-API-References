---
title: "WebExtensionBinding.Appref"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionBinding. تحصل وتعيّن مفتاح الربط المستخدم لربط الإدخال في هذه القائمة بالبيانات المرتبطة في المستند"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

يحصل ويضبط مفتاح الربط المستخدم لتعيين إدخال الربط في هذه القائمة مع البيانات المرتبطة في المستند.

```csharp
public string Appref { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyApprefDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة جديدة من WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // عيّن الخصائص بما في ذلك Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // عرض القيمة الحالية لـ Appref
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // تعديل قيمة Appref لإظهار أنها قابلة للقراءة/الكتابة
                binding.Appref = "Sheet1!C3:D4";
                Console.WriteLine("Updated Appref value: " + binding.Appref);
                
                Console.WriteLine("Appref property has been successfully demonstrated");
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


