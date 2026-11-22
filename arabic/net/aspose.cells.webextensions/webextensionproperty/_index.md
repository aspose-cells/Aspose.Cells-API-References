---
title: "الفئة WebExtensionProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WebExtensions.WebExtensionProperty. تمثل خاصية مخصصة لإضافة Office"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

يمثل خاصية مخصصة لإضافة Office Add-in.

```csharp
public class WebExtensionProperty
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | يحصل ويضبط اسم خاصية مخصصة. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | يحصل ويضبط قيمة خاصية مخصصة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ نسخة جديدة من WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // اضبط قيم الخصائص
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // عرض قيم الخصائص
                Console.WriteLine($"Property Name: {property.Name}");
                Console.WriteLine($"Property Value: {property.Value}");
                
                Console.WriteLine("WebExtensionProperty demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


