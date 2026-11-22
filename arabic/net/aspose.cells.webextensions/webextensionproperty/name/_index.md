---
title: "WebExtensionProperty.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionProperty. تحصل وتضبط اسم خاصية مخصص"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

يحصل ويضبط اسم خاصية مخصصة.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة من WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // تعيين وإظهار خاصية Name
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // تعديل وعرض الاسم المحدث
                property.Name = "UpdatedName";
                Console.WriteLine($"Modified Name: {property.Name}");
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


