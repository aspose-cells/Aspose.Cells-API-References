---
title: "WebExtensionProperty.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionProperty. تحصل وتضبط قيمة خاصية مخصصة"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

يحصل ويضبط قيمة خاصية مخصصة.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة من WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // تعيين وإظهار خاصية Value
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // تعديل وعرض القيمة المحدثة
                property.Value = "UpdatedValue456";
                Console.WriteLine($"Modified Value: {property.Value}");
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

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


