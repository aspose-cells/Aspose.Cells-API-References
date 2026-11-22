---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StreamProviderOptions. تحصل وتضبط نوع المورد المحمّل"
type: docs
url: /ar/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

يحصل ويضبط نوع مورد التحميل.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyResourceLoadingTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع خيارات StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // عرض سلوكيات تحميل الموارد المختلفة
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // توفير تدفق MemoryStream مخصص
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // تخطي التحميل باستخدام تدفق null
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // سلوك تحميل الملف الافتراضي
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // تنظيف
            options.Stream?.Dispose();
        }
    }
}
```

### انظر أيضًا

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


