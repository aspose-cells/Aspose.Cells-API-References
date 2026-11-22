---
title: "StreamProviderOptions.StreamProviderOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ StreamProviderOptions. يهيئ مثيلًا جديدًا من فئة StreamProviderOptions"
type: docs
url: /ar/net/aspose.cells/streamprovideroptions/streamprovideroptions/
---
## StreamProviderOptions(ResourceLoadingType, string) {#constructor_1}

يهيئ مثيلًا جديدًا من الفئة [`StreamProviderOptions`](../).

```csharp
public StreamProviderOptions(ResourceLoadingType loadingType, string defaultPath)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadingType | ResourceLoadingType | النوع لتحميل المورد المرتبط. |
| defaultPath | String | المسار الافتراضي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Microsoft.VisualBasic;
    using System;

    public class StreamProviderOptionsMethodCtorWithResourceLoadingTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("file1.xlsx");
            workbook.Settings.ResourceProvider = new StreamProvider();
            foreach (Shape shape in workbook.Worksheets[0].Shapes)
            {
                shape.ToImage("out.png", null);
            }            
        }
    }

    class StreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = File.OpenRead("example.jpg");
            options.ResourceLoadingType = ResourceLoadingType.UserProvided;
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

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## StreamProviderOptions() {#constructor}

يهيئ مثيلًا جديدًا من الفئة [`StreamProviderOptions`](../).

```csharp
public StreamProviderOptions()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class StreamProviderOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // إظهار المنشئ بدون معلمات
                StreamProviderOptions options = new StreamProviderOptions();
                Console.WriteLine("Parameterless constructor:");
                Console.WriteLine($"ResourceLoadingType: {options.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options.DefaultPath}");

                // إنشاء مصنف وحفظه باستخدام خيارات الدفق
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].PutValue("StreamProviderOptions Demo");
                
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                string outputDir = "custom_path/";
                saveOptions.StreamProvider = new ExportStreamProvider(outputDir);
                
                workbook.Save("StreamProviderOptionsDemo.html", saveOptions);
                Console.WriteLine("\nWorkbook saved with custom stream options");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StreamProviderOptions constructor demo: {ex.Message}");
            }
        }
    }

    internal class ExportStreamProvider : IStreamProvider
    {
        private string outputDir;

        public ExportStreamProvider(string dir)
        {
            outputDir = dir;
        }

        public void InitStream(StreamProviderOptions options)
        {
            if (options.DefaultPath == null)
            {
                options.Stream = new MemoryStream();
            }
            else
            {
                string path = outputDir + Path.GetFileName(options.DefaultPath);
                options.CustomPath = path;
                Directory.CreateDirectory(Path.GetDirectoryName(path));
                options.Stream = File.Create(path);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            if (options != null && options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### انظر أيضًا

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


