---
title: "StreamProviderOptions.Stream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StreamProviderOptions. تحصل/تضبط التدفق"
type: docs
url: /ar/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

يحصل/يضبط الدفق

```csharp
public Stream Stream { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyStreamDemo
    {
        public static void Run()
        {
            // إنشاء مثيل StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // الحالة 1: عندما لا يتم تعيين مسار افتراضي - استخدم MemoryStream
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // الحالة 2: محاكاة وجود مسار افتراضي - استخدم FileStream
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // تنظيف
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### انظر أيضًا

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


