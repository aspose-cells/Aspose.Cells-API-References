---
title: "StreamProviderOptions.CustomPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StreamProviderOptions. مسار URL المخصص للمستخدم يتم حفظه في ملف HTML المُولد للمصدر المشار إليه. إذا لم يحدده المستخدم سيتم استخدام DefaultPath. على سبيل المثال سيتم حفظ بيانات الورقة بواسطة المستخدم إلى d/sheet001.htm ويجب أن يكون عنوان URL المستخدم في ملف HTML الرئيسي هو d/sheet001.htm أو أي مسار نسبي صالح يمكن الوصول إليه من ملف HTML الرئيسي"
type: docs
url: /ar/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

المسار المخصص (URL) للمستخدم المحفوظ في ملف HTML المُولد للمصدر المشار إليه. إذا لم يحدده المستخدم، سيتم استخدام DefaultPath. على سبيل المثال، سيتم حفظ بيانات الورقة من قبل المستخدم إلى d:/sheet001.htm، ويجب أن يكون عنوان URL المستخدم في ملف HTML الرئيسي هو "d:/sheet001.htm" أو أي مسار نسبي صالح آخر يمكن الوصول إليه من ملف HTML الرئيسي.

```csharp
public string CustomPath { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // إعداد خيارات حفظ HTML مع موفر تدفق مخصص
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // إنشاء موفر تدفق مخصص باستخدام CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // احفظ المصنف
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // تحقق من أنه تم استخدام المسار المخصص
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // تنفيذ مبسط لموفر تدفق مخصص
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // سيتم وضع التنفيذ هنا
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // سيتم وضع التنفيذ هنا
        }
    }
}
```

### انظر أيضًا

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


