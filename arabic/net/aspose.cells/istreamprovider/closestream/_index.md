---
title: "IStreamProvider.CloseStream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IStreamProvider. تغلق الـstream"
type: docs
url: /ar/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

يغلق الدفق.

```csharp
public void CloseStream(StreamProviderOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | StreamProviderOptions |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نسخة من الفئة التجريبية التي تنفذ IStreamProvider
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // إنشاء StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // استدعاء طريقة CloseStream
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // عرض التأثير - في سيناريو حقيقي، سيغلق هذا الـstream
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // التنفيذ المطلوب من الواجهة
        }

        public void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### انظر أيضًا

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


