---
title: "StreamProviderOptions.DefaultPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StreamProviderOptions. عنوان المسار الافتراضي (pathURL) المحفوظ في ملف html المُولد للمصدر المشار إليه. على سبيل المثال، بيانات الورقة المحفوظة في xxx_files/sheet001.htm يجب أن يكون عنوان url المستخدم في ملف html الرئيسي مثل srcxxx_files/sheet001.htm"
type: docs
url: /ar/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

المسار الافتراضي (URL) المحفوظ في ملف html المُولد للمصدر المشار إليه. على سبيل المثال، يتم حفظ بيانات الورقة في xxx_files/sheet001.htm، يجب أن يكون عنوان url المستخدم في ملف html الرئيسي مثل "src=\"xxx_files/sheet001.htm\""

```csharp
public string DefaultPath { get; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            
            // إنشاء StreamProviderOptions مع ResourceLoadingType و DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // عرض استخدام DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // مثال على استخدام الخيارات مع دفق (عرض مبسط)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // إجراء عمليات مع الدفق
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


